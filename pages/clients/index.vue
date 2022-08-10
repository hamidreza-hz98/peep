<template>
    <v-container>
        <v-row>
            {{ $store.state.clients }}
            <SearchClient />
            <v-spacer />
            <ModalForm @onSubmit="addClient($event)" />
        </v-row>
        <ClientsTable :items="clients" />
    </v-container>
</template>

<script>
import ClientsTable from '../../components/ClientsTable/ClientsTable.vue'
import NewClientForm from '../../components/NewClientForm.vue'
import ModalForm from '../../components/ModalForm/ModalForm.vue'
import SearchClient from '../../components/SearchClient.vue'
export default {
    computed: {
        clients() {
            return this.$store.state.clients
        }
    },
    components: { ClientsTable, NewClientForm, ModalForm, SearchClient },

    data() {
        return {
            //clients: []
        }
    },
    methods: {
        // addClient(client) {
        //     const { firstName, lastName, mobile } = client
        //     const newClient = {
        //         ...client,
        //         name: firstName + ' ' + lastName,
        //         mobile: mobile,
        //         email: 'hamidreza.h@maticangroup.com',
        //         status: 'New',
        //     }
        //     this.clients.push(newClient)
        // }
        addClient(client) {
            const newClient = {
                ...client,

            }
            this.$store.commit('addClient', newClient)
        }
    }
}
</script>
