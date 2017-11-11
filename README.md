# vue-datepicker-local

Adjustments added so that it works within other vue components using scss.

### A Beautiful Datepicker Component For Vue2
* Lightweight (less than 4kb minified and gzipped)
* Only dependencies Vue
* Beautiful!

Forked from : https://github.com/weifeiyue/vue-datepicker-local

## Usage

### Install

```bash
$ npm install lsldigital/vue-datepicker-local
```

### ES6
```html
<template>
  <vue-datepicker-local v-model="time" />
</template>

<script>
import VueDatepickerLocal from 'vue-datepicker-local'

export default {
  components: {
    VueDatepickerLocal
  },
  data () {
    return {
      time: new Date()
    }
  }
}
</script>
```

### Props

| Prop           | Description                                      | Type       | Default            |
|:---------------|:-------------------------------------------------|:-----------|:-------------------|
| v-model        | dates to be manipulated                          | Date/Array | --                 |
| name           | name for input                                   | String     | --                 |
| inputClass     | custom class name for input                      | String     | --                 |
| popupClass     | custom class name for popup                      | String     | --                 |
| disabled       | determine whether the DatePicker is disabled     | Boolean    | false              |
| clearable      | clear the date                                   | Boolean    | false              |
| rangeSeparator | range separator                                  | String     | "~"                |
| format         | to set the date format                           | String     | "YYYY-MM-DD"       |


# French Locale

```
{
        dow: 0, // Sunday is the first day of the week
        hourTip: 'Select Hour', // tip of select hour
        minuteTip: 'Select Minute', // tip of select minute
        secondTip: 'Select Second', // tip of select second
        yearSuffix: '', // suffix of head year
        monthsHead: 'Janvier_Fevrier_Mars_Avril_Mai_Juin_Julliet_Aout_Septembre_Octobre_Novembre_Decembre'.split('_'), // months of head
        months: 'Jan_Fev_Mar_Avr_Mai_Jun_Jul_Aout_Sep_Oct_Nov_Dec'.split('_'), // months of panel
        weeks: 'Dim_Lun_Mar_Mer_Jeu_Ven_Sam'.split('_') // weeks
      }
      ```

## License
vue-datepicker-local is licensed under [The MIT License](LICENSE).
