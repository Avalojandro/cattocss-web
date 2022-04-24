<template>
    <div>
        <div class="text-white text-center text-5xl font-bold">
            {{animations[2].name}}
        </div>
        <div class="m-8 p-2">
            <pre>
                <code v-highlight class="css">
{{animations[2].code}}
                </code>
            </pre>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ComponentName',
    data() {
        return {
            // Data Here
            animations: [
              {
                name: 'Float',
                id: 0,
                code: `.float{
    transition: .5s, color .10s;
        -webkit-transition: .5s, color .10s;
        -moz-transition: .5s, color .10s;
}
.float:hover{
    box-shadow: 0 8px 8px 0 #bebbbc,0 8px 8px 0 #adadab;
    transform: translate(0px,5px);
        -webkit-transform: translate(0px,5px);
        -moz-transform:translate(0px,5px);
}`
              },
              {
                name: 'Rotate-180',
                id: 1,
                code: `.rotate-180{
    transition: .5s, color .10s;
        -webkit-transition: .5s, color .10s;
        -moz-transition: .5s, color .10s;
}
.rotate-180:hover{
    transform: rotate(180deg);
        -webkit-transform: rotate(180deg);
        -moz-transform: rotate(180deg);
}`
              },
              {
                name: 'Rotate-360',
                id: 0,
                code: `.rotate-360{
    transition: .5s, color .10s;
        -webkit-transition: .5s, color .10s;
        -moz-transition: .5s, color .10s;
}
.rotate-360:hover{
    transform: rotateZ(360deg);
        -webkit-transform: rotateZ(360deg);
        -moz-transform: rotateZ(360deg);
}`
              },
              {
                name: 'Flex',
                id: 0,
                code: `.flex{
    transition: .5s, color .10s;
        -webkit-transition: .5s, color .10s;
        -moz-transition: .5s, color .10s;
}
.flex:hover{
    transform: matrix(3.0, .5, 0, 1.0, 1.0, 1.0);
        -webkit-transform: matrix(3.0, .5, 0, 1.0, 1.0, 1.0);
        -moz-transform: matrix(3.0, .5, 0, 1.0, 1.0, 1.0);
}`
              },
              {
                name: 'TransLeft',
                id: 0,
                code: `.transLeft{
    transition: .5s, color .10s;
        -webkit-transition: .5s, color .10s;
        -moz-transition: .5s, color .10s;
}
.transLeft:hover{
    transform: translatex(-20px);
        -webkit-transform: translatex(-20px);
        -moz-transform: translatex(-20px);
}`
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
              {
                name: 'Float',
                id: 0,
                code: ``
              },
            ] 
        }
    },
    methods: {
        // Methods Here
        myMethod() {
            // Code Here
        }
    },
    computed: {
        // Computed Here
        myComputed() {
            // Code Here, remember return something
        }
    },
    watch: {
        // Watch Here
        myWatch(newVal, oldVal) {
            // Code Here on change value
        }
    },
}
</script>

<style>
/*!
  Theme: Tokyo-night-Dark
  origin: https://github.com/enkia/tokyo-night-vscode-theme
  Description: Original highlight.js style
  Author: (c) Henri Vandersleyen <hvandersleyen@gmail.com>
  License: see project LICENSE
  Touched: 2022
*/

/*  Comment */
.hljs-meta,
.hljs-comment {
  color: #565f89;
}

/* Red */
/*INFO: This keyword, HTML elements, Regex group symbol, CSS units, Terminal Red */
.hljs-tag,
.hljs-doctag,
.hljs-selector-id,
.hljs-selector-class,
.hljs-regexp,
.hljs-template-tag,
.hljs-selector-pseudo,
.hljs-selector-attr,
.hljs-variable.language_,
.hljs-deletion {
  color: #ff6600;
}

/*Orange */
/*INFO: Number and Boolean constants, Language support constants */
.hljs-variable,
.hljs-template-variable,
.hljs-number,
.hljs-literal,
.hljs-type,
.hljs-params,
.hljs-link {
  color: #ff00c8;
}


/*  Yellow */
/* INFO:  	Function parameters, Regex character sets, Terminal Yellow */
.hljs-built_in, 
.hljs-attribute {
  color: #00f7ff;
}
/* cyan */
/* INFO: Language support functions, CSS HTML elements */
.hljs-selector-tag {
  color: #2ac3de;
}

/* light blue */
/* INFO: Object properties, Regex quantifiers and flags, Markdown headings, Terminal Cyan, Markdown code, Import/export keywords */
.hljs-keyword,
  .hljs-title.function_,
.hljs-title,
.hljs-title.class_,
.hljs-title.class_.inherited__,
.hljs-subst,
.hljs-property {color: #7dcfff;}

/*Green*/
/* INFO: Object literal keys, Markdown links, Terminal Green */
.hljs-selector-tag { color: #73daca;}


/*Green(er) */
/* INFO: Strings, CSS class names */
.hljs-quote,
.hljs-string,
.hljs-symbol,
.hljs-bullet,
.hljs-addition {
  color: #9ece6a;
}

/* Blue */
/* INFO:  	Function names, CSS property names, Terminal Blue */
.hljs-code,
.hljs-formula,
.hljs-section {
  color: #7aa2f7;
}



/* Magenta */
/*INFO: Control Keywords, Storage Types, Regex symbols and operators, HTML Attributes, Terminal Magenta */
.hljs-name,
.hljs-keyword,
.hljs-operator,
.hljs-keyword,
.hljs-char.escape_,
.hljs-attr {
  color: #bb9af7;
}

/* white*/
/* INFO: Variables, Class names, Terminal White */
.hljs-punctuation {color: #c0caf5}

.hljs {
  @apply bg-gray-800;
  @apply rounded-xl;
  color: #9aa5ce;
}

.hljs-emphasis {
  font-style: italic;
}

.hljs-strong {
  font-weight: bold;
}
</style>