CKEditor 5 classic editor build
========================================

First, install the build from npm:

```bash
npm install --save ckeditor5-build-from-source
```

And use it in your website:

```html
<template>
	<ckeditor 
        v-model="somevalue"         
        :editor="editor" 
        :config="editorConfig" />
</template>
<script>
import CKEditor from '@ckeditor/ckeditor5-vue'
Vue.use( CKEditor );

require('ckeditor5-build-from-source')

export default {
    data(){
        return {
            editor: window.ClassicEditor,
            editorConfig: {
            	//the editor config
            }
        }
    }
}
</script>
```
