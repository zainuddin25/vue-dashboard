<template>
  <div
    class="w-full bg-slate-100 h-[10%] flex justify-between items-center px-8"
  >
    <span class="font-light text-lg"
      >Good Morning, <span class="font-bold text-xl">Admin</span></span
    >
    <div class="flex items-center gap-10">
      <div class="flex items-center gap-3">
        <div class="tooltip relative">
          <img class="cursor-pointer" src="/img/Bell_pin.svg" alt="Bell Icon" />
          <span
            class="w-[100px] duration-100 tooltip-text absolute -bottom-10 left-1/2 -translate-x-1/2 py-2 px-4 bg-slate-300 text-white text-center text-sm rounded-lg opacity-0 pointer-events-none"
          >
            Notification
          </span>
        </div>
        <div class="tooltip relative">
          <img
            class="cursor-pointer"
            src="/img/setting_line.svg"
            alt="Bell Icon"
          />
          <span
            class="w-[100px] duration-100 tooltip-text absolute -bottom-10 left-1/2 -translate-x-1/2 py-2 px-4 bg-slate-300 text-white text-center text-sm rounded-lg opacity-0 pointer-events-none"
          >
            Setting
          </span>
        </div>
        <div class="tooltip relative">
          <img
            class="cursor-pointer"
            src="/img/Sign_out_squre.svg"
            alt="Log Out Icon"
          />
          <span
            class="w-[100px] duration-100 tooltip-text absolute -bottom-10 left-1/2 -translate-x-1/2 py-2 px-4 bg-slate-300 text-white text-center text-sm rounded-lg opacity-0 pointer-events-none"
          >
            Logout
          </span>
        </div>
      </div>
      <div>
        <img
          src="https://images.unsplash.com/photo-1677492750297-bf465600cb04?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=1974&q=80"
          class="w-10 h-10 rounded-full"
        />
      </div>
    </div>
  </div>
</template>

<style>
.tooltip-text {
  visibility: hidden; 
}

.tooltip:hover .tooltip-text {
  visibility: visible;
  opacity: 1;
  pointer-events: auto;
}
</style>