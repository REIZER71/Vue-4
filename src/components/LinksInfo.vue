<script>
export default {
    data: () => ({
      items: [
        {
          title: 'Youtube',
          disabled: false,
          href: 'https://www.youtube.com/watch?v=K0HSD_i2DvA',
        },
        {
          title: 'Yandex Music',
          disabled: false,
          href: 'https://music.yandex.ru/album/49357/track/353713?utm_source=promodj&utm_medium=track&utm_campaign=product',
        },
        {
          title: 'VK music',
          disabled: false,
          href: 'https://vk.com/audio-2001242153_106242153',
        },
      ],
    }),
  }
</script>
<template>
 <v-card-item class="bg-black">
      <v-card-title>
       Links
      </v-card-title>
      </v-card-item>
    <v-divider></v-divider>
    <br>

<v-breadcrumbs
      :items="items"
      divider="/"
    ></v-breadcrumbs>
</template>