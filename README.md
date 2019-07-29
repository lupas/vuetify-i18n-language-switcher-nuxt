# Vuetify-18n-Language-Switcher-Nuxt

> **Important:**
> This package is just used for personal / test-purposes and not really meant for production or distribution (yet). If you plan to use it in your project, do so on your own risk. Feel free to use it though and suggest improvements :-)

Easily adds a language switcher to a Nuxt+Vuetify+I88n App similar to the one on Vuetifyjs.com

<p align="center"><img align="center" height="300px" src="https://github.com/lupas/vuetify-i18n-language-switcher-nuxt/blob/master/docs/exampleScreenshot.png?raw=true"/></p>

# How to install?

```js
npm i vuetify-i18n-language-switcher-nuxt
```

# How to use in your project?

Import the component in any .vue file like so:

```js
...
components: {
  VuetifyI18nLanguageSwitcherNuxt: () =>
    import('vuetify-i18n-language-switcher-nuxt')
}
...
```

# Example Usage

HTML:

```html
<VuetifyI18nLanguageSwitcherNuxt :languages="languages" />
```

Script:

```js
export default {
  components: {
    VuetifyI18nLanguageSwitcherNuxt: () =>
      import('vuetify-i18n-language-switcher-nuxt')
  },
  data() {
    return {
      languages: [
        {
          id: 'en',
          title: 'English',
          flagSrc: 'https://cdn.vuetifyjs.com/images/flags/us.png'
        },
        {
          id: 'kr',
          title: 'Korean',
          flagSrc: 'https://cdn.vuetifyjs.com/images/flags/kr.png'
        }
      ]
    }
  }
}
```
