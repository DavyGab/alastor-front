<template>
    <div class="card">
        <div class="card-body">
            <h4 class="card-title">Data Table</h4>
            <h6 class="card-subtitle">Data table example</h6>
            <div class="table-responsive m-t-40">
                <table id="myTable" class="table table-bordered table-striped">
                    <thead>
                        <tr>
                            <th>Nom</th>
                            <th>Dossier</th>
                            <th>Echéance</th>
                            <th>Responsable</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr v-for="deadline in deadlines">
                            <td>{{ deadline.name }}</td>
                            <td>{{ deadline.topic }}</td>
                            <td>{{ deadline.date }}</td>
                            <td>{{ deadline.responsible }}</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>
        </div>
</template>

<script>
export default {
    name: 'TableDeadline',
    data () {
        return {
            deadlines : [
                {
                    name: 'FAQ',
                    topic: 'WebSite',
                    date: '13/01/1991',
                    responsible: 'Davy Gabison'
                },
                {
                    name: 'TOTO List',
                    topic: 'WebSite',
                    date: '01/01/1991',
                    responsible: 'Adé'
                }
            ]
        }
    }
}
</script>
<style>
</style>