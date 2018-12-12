<template>
<v-container fluid="" px-0 pt-1>
    <v-layout column="" px-0>
        <v-flex lg12 pa-0>
            <InfoContract></InfoContract>
        </v-flex>
        <v-flex lg12 pa-0>
            <TabFunc></TabFunc>
        </v-flex>
    </v-layout>

</v-container>
</template>

<script>
import InfoContract from '@/components/InfoPanel/InfoContract'
import TabFunc from '@/components/FuncPanel/TabFunc'
export default {
    name: 'Main',
    components: {
        InfoContract,
        TabFunc
    }
}
</script>

<style>

</style>
