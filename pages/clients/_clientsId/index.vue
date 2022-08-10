<template>
    <v-container>
        <v-row>
            <v-col cols="3">
                <v-btn>Edit</v-btn>
                <h3>Hessa Al Halman</h3>
                <v-btn color="primary">New Appointment</v-btn>
                <br />
                <br />
                <v-btn-toggle>
                    <v-btn>Block</v-btn>
                    <v-btn>VIP</v-btn>
                </v-btn-toggle>
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
                <ClientInfoTypo title="Mobile" value="09121212147" />
            </v-col>
            <v-col cols="9">
                <v-row>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="95px" width="376px">KD 0</v-sheet>
                    </v-col>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="95px" width="376px">KD 0</v-sheet>
                    </v-col>
                </v-row>
                <v-row>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="88px" width="167px">All Bookings</v-sheet>
                    </v-col>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="88px" width="167px">Completed</v-sheet>
                    </v-col>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="88px" width="167px">Cancelled</v-sheet>
                    </v-col>
                    <v-col>
                        <v-sheet color="white" elevation="1" height="88px" width="167px">No Shows</v-sheet>
                    </v-col>
                </v-row>
                <v-tabs>
                    <v-tab>Item One</v-tab>
                    <v-tab>Item Two</v-tab>
                    <v-tab>Item Three</v-tab>

                    <v-tab-item>
                        <v-card>
                            <v-card-text>
                                <p>This is Item one</p>
                            </v-card-text>
                        </v-card>
                    </v-tab-item>
                    <v-tab-item>
                        <v-card>
                            <v-card-text>
                                <p>This is Item two</p>
                            </v-card-text>
                        </v-card>
                    </v-tab-item>
                    <v-tab-item>
                        <v-card>
                            <v-card-text>
                                <p>This is Item three</p>
                            </v-card-text>
                        </v-card>
                    </v-tab-item>
                </v-tabs>
            </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {
    mounted() {
        const clientPhone = this.$route
        console.log(clientPhone);
    },
}
</script>