<template>
    <li class="newbie-contributor">
        <div class="avatar">
            <img :src="contributor.avatar_url" />
        </div>
        <div :class="renderClasses"><b>#{{ contributor.rank }}</b></div>
        <div class="name">{{ contributor.login }}</div>
        <div class="contributions">{{ contributor.contributions }} contrib.</div>
    </li>
</template>

<script>
import Avatar from './Avatar.vue'

export default{
    name: 'avatar-item',
    extends: Avatar,
    props: ['contributor', 'category']
}
</script>
