<template>
  <q-layout view="hHh lpR fFf">
    <DesktopNAV />
    <MobileNAV />

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
export default {
  name: 'Main',
  components: {
    DesktopNAV: () => import('components/navigation/desktop/Header'),
    MobileNAV: () => import('components/navigation/mobile/Menu'),
  },
};
</script>
