<template lang="pug">
  component-view(v-bind:doc="doc")
</template>

<script>
  export default {
    data () {
      return {
        doc: {
          component: 'subheader',
          edit: 'SubheaderView',
          title: 'Subheaders',
          desc: 'The <code>v-subheader</code> component is used to separate sections of lists.',
          examples: [
            { header: 'List subheaders', file: 'subheaders/list', desc: 'Subheaders work great with lists for describing the information below.' },
            { header: 'Grid subheaders', file: 'subheaders/grid', desc: 'A subheader can add context to what a user is looking at.' },
            { header: 'Menu subheaders', file: 'subheaders/menu', desc: 'Using a subheader can help separate different types of actions.' }
          ],
          props: {
            'v-subheader': {
              shared: ['theme'],
              params: [
                [
                  'inset',
                  'Boolean',
                  'False',
                  'Adds identation (72px)'
                ]
              ]
            }
          }
        }
      }
    }
  }
</script>
