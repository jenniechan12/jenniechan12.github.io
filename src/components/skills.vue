<template lang="pug">
    v-container(fluid)
        v-row.text-center(align='center' justify='center')
            v-col(cols='12' md='8')
                v-card(flat color='transparent' style='border-color: #eb6b6f !important; border-style: solid;')
                    v-container(fluid)
                        v-row(align='center' justify='center')
                            v-col(cols='12' md='4')
                                //- Game Developer
                                v-card(flat color='transparent')
                                    v-card-text
                                        v-icon(size='64' color='#eb6b6f') fa-gamepad
                                        h2.my-2 Game Developer

                            v-col(cols='12' md='4')
                                //-Front End Developer 
                                v-card(flat color='transparent')
                                    v-card-text
                                        v-icon(size='64' color='#eb6b6f') fa-laptop-code
                                        h2.my-2 Front End Developer

                            v-col(cols='12' md='4')
                                //-Front End Developer 
                                v-card(flat color='transparent')
                                    v-card-text
                                        v-icon(size='64' color='#eb6b6f') fa-laptop-code
                                        h2.my-2 Front End Developer
</template>
<script>
export default {
  name: "Skills",
};
</script>
