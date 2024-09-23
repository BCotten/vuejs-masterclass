<script setup lang="ts"></script>

<template>
  <aside
    class="flex flex-col h-screen gap-2 border-r fixed bg-muted/40 lg:w-52 w-16 transition-[width]"
  >
    <div class="flex items-center justify-between h-16 gap-1 px-2 border-b lg:px-4 shrink-0">
      <button variant="outline" size="icon" class="w-8 h-8">
        <iconify-icon icon="lucide:menu" />
      </button>

      <button variant="outline" size="icon" class="w-8 h-8">
        <iconify-icon icon="lucide:plus" />
      </button>
    </div>

    <nav class="relative flex flex-col justify-between h-full gap-2">
      <div>
        <RouterLink
          to="/"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:house" />
          <span class="hidden lg:block text-nowrap">Dashboard</span>
        </RouterLink>
        <RouterLink
          to="/projects"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:building-2" />
          <span class="hidden lg:block text-nowrap">Projects</span>
        </RouterLink>
        <RouterLink
          to="/tasks"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:badge-check" />
          <span class="hidden lg:block text-nowrap">My Tasks</span>
        </RouterLink>
      </div>

      <div class="py-3 text-center border-y bg-background">
        <RouterLink
          to="/profile"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:user" />
          <span class="hidden lg:block text-nowrap">Profile</span>
        </RouterLink>
        <RouterLink
          to="/settings"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:settings" />
          <span class="hidden lg:block text-nowrap">Settings</span>
        </RouterLink>
        <RouterLink
          to="/signout"
          class="flex items-center justify-center gap-3 px-4 py-2 mx-2 transition-colors rounded-lg hover:text-primary lg:justify-normal text-muted-foreground"
        >
          <iconify-icon icon="lucide:log-out" />
          <span class="hidden lg:block text-nowrap">Sign out</span>
        </RouterLink>
      </div>
    </nav>
  </aside>
</template>
