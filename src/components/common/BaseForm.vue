<template>
<form>
  <searvice-select></searvice-select>
  <site-check></site-check>
  <unitary-check></unitary-check>
  <device-check></device-check>
  <term-check></term-check>
  <date-check></date-check>
</form>
</template>

<script>
import SearviceSelect from '../form/SearviceSelect'
import SiteCheck from '../form/SiteCheck'
import UnitaryCheck from '../form/UnitaryCheck'
import DeviceCheck from '../form/DeviceCheck'
import TermCheck from '../form/TermCheck'
import DateCheck from '../form/DateCheck'

export default {
  components: {
    SearviceSelect,
    SiteCheck,
    UnitaryCheck,
    DeviceCheck,
    TermCheck,
    DateCheck
  }
}
</script>