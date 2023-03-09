<template>
    <div class="grid grid-cols-4 gap-4">
        <CardDashboardCard v-for="(data, index) in dataCard" :key="index" :img="data.img" :desc="data.desc" :total="data.total" :title="data.title" />
    </div>
    <div class="w-full mt-6 flex gap-4 relative">
        <div class="w-3/4">
            <span class="text-2xl font-bold">Users Table</span>
            <TableDashboardTable />
        </div>
        <div class="w-1/4">
            <span class="text-2xl font-bold">News Waiting Approve</span>
            <CardNewsWaitingApprove v-for="(data, index) in dataCardNews" :key="index" :img="data.img" :title-news="data.titleNews" :news-description="data.newsDescription" :user-created="data.userCreated" :date-created="data.dateCreate" />
        </div>
    </div>
</template>

<script setup>
    const dataCard = [
        {
            img: '/img/Group.svg',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            total: '30',
            title: 'Users'
        },
        {
            img: '/img/Ticket_use.svg',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            total: '193',
            title: 'Products'
        },
        {
            img: '/img/In.svg',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            total: '$ 201.00',
            title: 'Profit'
        },
        {
            img: '/img/Out.svg',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit.',
            total: '$ 0',
            title: 'Loss'
        },
    ]
    
    const dataCardNews = [
        {
            img: 'https://images.unsplash.com/photo-1566073771259-6a8506099945?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80',
            titleNews: 'Burhan Buat Hotel Baaru',
            newsDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, accusantium? Qui dolore, voluptatum magnam praesentium, quidem culpa possimus ratione accusamus aspernatur iure eum tempore corporis, error laboriosam voluptas beatae libero!',
            userCreated: 'Asep Dadang',
            dateCreate: '01 03 2023'
        },
        {
            img: 'https://images.unsplash.com/photo-1566073771259-6a8506099945?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80',
            titleNews: 'Burhan Buat Hotel Baaru',
            newsDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, accusantium? Qui dolore, voluptatum magnam praesentium, quidem culpa possimus ratione accusamus aspernatur iure eum tempore corporis, error laboriosam voluptas beatae libero!',
            userCreated: 'Asep Dadang',
            dateCreate: '01 03 2023'
        },
        {
            img: 'https://images.unsplash.com/photo-1566073771259-6a8506099945?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80',
            titleNews: 'Burhan Buat Hotel Baaru',
            newsDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, accusantium? Qui dolore, voluptatum magnam praesentium, quidem culpa possimus ratione accusamus aspernatur iure eum tempore corporis, error laboriosam voluptas beatae libero!',
            userCreated: 'Asep Dadang',
            dateCreate: '01 03 2023'
        },
        {
            img: 'https://images.unsplash.com/photo-1566073771259-6a8506099945?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1170&q=80',
            titleNews: 'Burhan Buat Hotel Baaru',
            newsDescription: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Et, accusantium? Qui dolore, voluptatum magnam praesentium, quidem culpa possimus ratione accusamus aspernatur iure eum tempore corporis, error laboriosam voluptas beatae libero!',
            userCreated: 'Asep Dadang',
            dateCreate: '01 03 2023'
        },
    ]

</script>