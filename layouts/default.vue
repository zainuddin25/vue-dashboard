<style>
/* Style untuk scrollbar */
#scroll-bar-hidden::-webkit-scrollbar {
  width: 8px; /* Lebar scrollbar */
}

#scroll-bar-hidden::-webkit-scrollbar-track {
  background-color: #f5f5f5; /* Warna track scrollbar */
}

#scroll-bar-hidden::-webkit-scrollbar-thumb {
  background-color: #ccc; /* Warna thumb scrollbar */
  border-radius: 4px; /* BorderRadius untuk thumb */
}

#scroll-bar-hidden::-webkit-scrollbar-thumb:hover {
  background-color: #999; /* Warna thumb scrollbar saat dihover */
}
</style>

<template>
    <div class="flex h-screen w-screen">
        <div class="w-[20%] bg-slate-100 h-full">
            <LayoutSidebar />
        </div>
        <div class="w-[80%] bg-slate-50">
            <LayoutHeader/>
            <div class="w-full h-[80%] bg-slate-100 px-8 py-4 overflow-scroll overflow-x-hidden" id="scroll-bar-hidden">
                <slot />
            </div>
            <LayoutFooter/>
        </div>
    </div>
</template>