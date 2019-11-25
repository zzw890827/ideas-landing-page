<template>
  <div
    :id="ids"
    data-parallax="true"
    :style="'background:url(' + bgImage + ')'"
    :class="classNames"
  >
    <slot />
  </div>
</template>

<script>
export default {
  name: 'ParallaxStyle1',
  // eslint-disable-next-line vue/require-prop-types
  props: ['ids', 'bgImage', 'classNames']
}
</script>
