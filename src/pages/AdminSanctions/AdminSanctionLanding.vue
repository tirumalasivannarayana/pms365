<template>
<div class="md-layout">
    <div class="md-layout-item md-size-100">
        <nav-tabs-card>
            <template slot="content">
                <span class="md-nav-tabs-title">Create:</span>
                <md-tabs md-sync-route class="md-primary" md-alignment="left">
                    <md-tab id="tab-home" md-label="AdminSanction">
                    </md-tab>
                    <md-tab id="tab-pages" md-label="Project">

                    </md-tab>
                    <md-tab id="tab-posts" md-label="Work" >

                    </md-tab>
                    <md-tab id="tab-posts" md-label="Tech Sanction" >

                    </md-tab>
                    <md-tab id="tab-posts" md-label="Work" md-icon="cloud">
                        <nav-tabs-table></nav-tabs-table>
                    </md-tab>

                </md-tabs>
            </template>
        </nav-tabs-card>
    </div>
</div>
</template>
<script>


    import NavTabsCard from "../../components/Cards/NavTabsCard";
    import NavTabsTable from "../../components/Tables/NavTabsTable";

    export default{
        components: {
            NavTabsCard,
            NavTabsTable
        }
    }
</script>