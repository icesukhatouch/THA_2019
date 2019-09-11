<template>
    <b-container>
        <b-row>
            <b-col class="topic">AGENDA</b-col>
            <b-col class="d-flex align-items-center">
                <div class="headline"></div>
            </b-col>
        </b-row>
        <div class="table-agenda">
            <b-tabs content-class="mt-3" align="center">
                <b-tab active>
                    <template slot="title">
                        <b-spinner type="grow" small></b-spinner> 
                        <h1>DAY1</h1> 
                        <p>20 December 2019</p>
                    </template>
                    <b-tabs content-class="mt-3" align="center">
                        <b-tab active>
                            <template slot="title">
                                <h4>Grand Stage and Expo</h4> 
                            </template>
                            <b-table hover responsive :items="items" :fields="fields"></b-table>
                        </b-tab>
                        <b-tab>
                            <template slot="title">
                                <h4>Conference I</h4> 
                                <p>MR 214-216</p>
                            </template>
                            <b-table hover responsive :items="items" :fields="fields"></b-table>
                        </b-tab>
                        <b-tab>
                            <template slot="title">
                                <h4>Conference II</h4> 
                                <p>GH 203</p>
                            </template>
                            <b-table hover responsive :items="items" :fields="fields"></b-table>
                        </b-tab>
                        <b-tab>
                            <template slot="title">
                                <h4>Conference III</h4> 
                                <p>MR 222-223</p>
                            </template>
                            <b-table hover responsive :items="items" :fields="fields"></b-table>
                        </b-tab>
                    </b-tabs>
                </b-tab>

                <b-tab>
                    <template slot="title">
                        <b-spinner type="grow" small></b-spinner> 
                        <h1>DAY2</h1> 
                        <p>21 December 2019</p>
                    </template>
                    <p>I'm the second tab</p>
                </b-tab>
                <b-tab>
                    <template slot="title">
                        <b-spinner type="grow" small></b-spinner> 
                        <h1>DAY3</h1> 
                        <p>22 December 2019</p>
                    </template>
                    <p>I'm a disabled tab!</p>
                </b-tab>
            </b-tabs>
        </div>
    </b-container>
</template>



<script>
export default {
    data() {
        return {
            fields: {
                time: {
                    label: ""
                },
                description: {
                    label: ""
                }
            },
            items: [
                { time: 40, description: 'Dickerson' },
                { time: 21, description: 'Larsen' },
                { time: 89, description: 'Geneva'},
                { time: 38, description: 'Jami'}
            ]
        }
    }
}
</script>


<style scoped>
    .topic {
        font-size: 5rem;
        color: #FDD738;
    }
    .headline {
        border: 2px white solid;
        width: 40rem;
    }
    .table-agenda {
        width: 100%;
    }
</style>
