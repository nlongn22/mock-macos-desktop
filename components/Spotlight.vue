<template>
    <Dialog class="spotlight">
        <Icon
            name="spotlight"
            class="spotlight__icon"
        />
        <input
            placeholder="Spotlight Search"
            class="spotlight__input"
        >
    </Dialog>
</template>

<script setup lang="ts">
</script>

<style lang="scss" scoped>
.spotlight {
    inset-inline-start: 50%;
    inset-block-start: 25vh;
    transform: translate(-50%, -50%);
    inline-size: r(675);
    display: flex;
    align-items: center;
    height: min-content;
    column-gap: $space-1;
    padding-inline: r(14);
    padding-block: $space-3;
    border-radius: $border-radius-xl;
    border-color: rgba($color-border, $opacity-low);
    box-shadow: rgba($color-foreground, $opacity-low) 0 r(20) r(30);
}

.spotlight__icon {
    inline-size: $space-6;
    block-size: $space-6;
    color: $color-gray-100;
}

.spotlight__input {
    inline-size: 100%;
    font-size: $space-6;
    font-weight: $font-weight-medium;

    &::placeholder {
        color: rgba($color-gray-200, $opacity-medium);
    }

    @include has-hover {
        cursor: revert;
    }
}
</style>
