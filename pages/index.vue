<template>
  <div class="border border-red-500 m-4 text-center mx-auto w-1/4">Nothing is here..</div>
</template>

<script lang="ts" setup>
onBeforeMount(() => {
  const route = useRoute();
  const router = useRouter();
  if (route.fullPath === "/") return router.push("/sample_1");
});
</script>
