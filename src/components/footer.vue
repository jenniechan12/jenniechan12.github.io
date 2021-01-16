<template lang="pug">
    v-footer(padless absolute)
        v-card.text-center(flat tile color='#eb6b6f' width='100%')
            v-card-text
                v-btn.ma-4(v-for='(item, index) in socialMedia' :key='index' outlined icon dark color='#7c3f58')
                    v-icon {{ item.icon }}
                v-divider.mx-auto(color='#7c3f58' width='60%')
                div.ma-4(style='color: #7c3f58') &#169;	created by me - <strong> {{ 2020 }} </strong>
</template>
<script>
export default {
  name: "Footer",

  data() {
    return {
      socialMedia: [{ icon: "fa-linkedin" }, { icon: "fa-github" }],
    };
  },
};
</script>
