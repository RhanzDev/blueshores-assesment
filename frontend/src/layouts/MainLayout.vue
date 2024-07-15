<template>
  <div class="signup-flow">
    <StepsIndicatorComponent :percentage="0" :startingPointLabel="'Setup An Account'"/>
    <div class="container">
      <div class="form-container">
      </div>
      <div class="marketing-container">
        <div class="diagonal"></div>
      </div>
      <PhoneNumberComponent :label="'Have any concerns or immediate booking needs?'" :phone-numbers="['0800-PHONE-ME', '0700-PHONE']" />
      
    </div>
  </div>
</template>

<script>
import StepsIndicatorComponent from 'components/StepsIndicatorComponent.vue';
import PhoneNumberComponent from 'components/PhoneNumberComponent.vue';
import scss 	from '../styles/styles.scss';
export default {
  components: { StepsIndicatorComponent, PhoneNumberComponent },
};
</script>
