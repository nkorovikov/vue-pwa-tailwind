<template>
    <a
        v-if="updateExists"
        @click="refreshApp"
        href="#"
        class="block px-4 py-2 text-sm text-gray-700 hover:bg-gray-100"
        role="menuitem"
    >
        Update app</a
    >
</template>

<script>
import update from '../domain/abstract/mixins/update'

export default {
    name: 'Home',
    mixins: [update],
}
</script>
