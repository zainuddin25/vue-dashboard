<template>
    <div class="relative overflow-x-auto shadow-md sm:rounded-lg mt-4">
        <table class="w-full text-sm text-left text-gray-500 dark:text-gray-400">
            <thead class="text-xs text-gray-700 uppercase bg-gray-50">
                <tr>
                    <th scope="col" class="px-6 py-3">
                        Username
                    </th>
                    <th scope="col" class="px-6 py-3">
                        <div class="flex items-center">
                            ID User
                        </div>
                    </th>
                    <th scope="col" class="px-6 py-3">
                        <div class="flex items-center">
                            Join AT
                        </div>
                    </th>
                    <th scope="col" class="px-6 py-3">
                        <div class="flex items-center">
                            Role
                        </div>
                    </th>
                    <th scope="col" class="px-6 py-3">
                        <div class="flex items-center">
                            Action
                        </div>
                    </th>
                </tr>
            </thead>
            <tbody>
                <tr class="border-b" v-for="(data, index) in dataUsers" :key="index" :class="index % 2 === 0 ? 'bg-white' : 'bg-gray-50'">
                    <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                        {{ data.username }}
                    </th>
                    <td class="px-6 py-4">
                        {{ data.idUser }}
                    </td>
                    <td class="px-6 py-4">
                        {{ data.joinAt }}
                    </td>
                    <td class="px-6 py-4">
                        {{ data.role }}
                    </td>
                    <td class="px-6 py-4 flex items-center">
                        <img src="/img/Trash.svg" alt="trash-icon" class="pr-2" /> |
                        <img src="/img/Edit.svg" alt="trash-icon" class="pl-2" />
                    </td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script setup>

const dataUsers = [
    {
        id: '1',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
    {
        id: '2',
        username : 'Nuks',
        idUser: '10ka3',
        joinAt: '09 03 2023',
        role: 'Admin Saller',
    },
]

</script>