<template>
<div>
  <searvice-select></searvice-select>
  <site-check></site-check>
  <unitary-check></unitary-check>
  <device-check></device-check>
  <index-check></index-check>
  <term-check></term-check>
  <date-check></date-check>
</div>
</template>

<script>
import SearviceSelect from '../form/SearviceSelect'
import SiteCheck from '../form/SiteCheck'
import UnitaryCheck from '../form/UnitaryCheck'
import DeviceCheck from '../form/DeviceCheck'
import IndexCheck from '../form/IndexCheck'
import TermCheck from '../form/TermCheck'
import DateCheck from '../form/DateCheck'

export default {
  components: {
    SearviceSelect,
    SiteCheck,
    UnitaryCheck,
    DeviceCheck,
    IndexCheck,
    TermCheck,
    DateCheck
  }
}
</script>