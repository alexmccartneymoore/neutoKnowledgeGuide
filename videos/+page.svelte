<script lang="ts">
    import fs from 'fs'; 
    import Markdoc from '@markdoc/markdoc';
    import {text} from './text.js';

    const parsed = Markdoc.parse(text);
    const content = Markdoc.transform(parsed /* config*/);      //config stage possible
    let html = Markdoc.renderers.html(content);

</script>
 
{@html html}
