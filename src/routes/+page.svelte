<script lang="ts">
// https://www.npmjs.com/package/svelte-persisted-store

import { get } from 'svelte/store'
import { preferences } from './stores'

preferences.set({
    theme: 'ligth',
    pane: '100%',
  }) // set value

$: console.log(get(preferences))
</script>

