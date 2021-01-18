<template lang="pug">
    //- v-container(fluid)
        v-row.text-center(align='center' justify='center')
            v-col(cols='12' md='8')
                v-card(flat color='transparent')
                    v-container(fluid)
                        v-row(align='center' justify='center')
                            v-col(cols='12')
                                h1.font-weight-medium ----- RECENT WORKS -----
                            v-col(cols='12' md='4')
                                //- Game Developer
                                v-hover(v-slot='{ hover }')
                                    v-card(flat)
                                        v-img(:aspect-ratio='16/9' src='http://leapcaller.com/tempheader.png?b95891978678b415a21cfc6651342522')
                                            v-expand-transition
                                                div.d-flex.transition-fast-in-fast-out.v-card--reveal.display-3.white--text(v-if='hover' style='height: 100%; background-color: rgb(124 63 88 / 84%);')

</template>
<script>
export default {
  name: "RecentWorks",
};
</script>
