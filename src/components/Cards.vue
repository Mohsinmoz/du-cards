<template>
  <v-sheet class="mx-auto" elevation="0" max-width="1266">
    <v-slide-group v-model="model" class="pa-4" active-class="success" show-arrows>
      <v-slide-item class="rounded-lg pa-4 pl-5 pb-11" v-for="(item, i) in items" :key="i">
        <v-card class="ma-2" elevation="2" width="300">
          <v-card-text class="pa-0">
            <div class="du-card--elem mb-4 pb-4">
              <span class="d-block subtitle-2 pink--text text--darken-2">{{ item.YouPay }}</span>
              <span class="d-inline title font-weight-bold pink--text text--darken-2">{{ item.Price }}</span> <span class="subtitle-2 pink--text text--darken-2">{{ item.PerMonth }}</span>
              <span class="d-block caption black--text">{{ item.Months }}</span>
            </div>
            <div class="du-card--elem mb-4 pb-4">
              <h2>
                <span class="d-block subtitle-2 light-blue--text text--darken-1">{{ item.SubTitle }}</span>
                <span class="headline font-weight-bold light-blue--text text--darken-1">{{ item.Title }}</span>
              </h2>
            </div>
            <div class="du-card--elem mb-4 pb-4">
              <div class="d-flex align-center pb-2">
                <span class="headline font-weight-bold black--text pr-6">{{ item.Data }}</span> <span class="caption black--text">{{
                  item.DataTitle }}</span>
              </div>
              <div class="d-flex align-center">
                <span class="headline font-weight-bold black--text pr-6">{{ item.Minutes }}</span> <span class="caption black--text">{{
                  item.MinutesTitle }}</span>
              </div>
            </div>
            <div class="du-card--elem mb-4 pb-4">
              <span class="du-card__benefit test d-block pb-1 caption black--text">{{ item.BenefitOne }}</span>
              <span class="du-card__benefit d-block pb-1 caption black--text">{{ item.BenefitTwo }}</span>
              <span class="du-card__benefit d-block pb-1 caption black--text">{{ item.BenefitThree }}</span>
              <span class="du-card__benefit d-block pb-1 caption black--text">{{ item.BenefitFour }}</span>
              <span class="du-card__benefit d-block pb-1 caption black--text">{{ item.BenefitFive }}</span>
              <span class="du-card__benefit d-block caption black--text">{{ item.BenefitSix }}</span>
            </div>
            <div class="du-card--elem mb-4 pb-4">
              <div class="d-block mb-2">
                <span class="du-card__limited d-inline pt-1 pb-1 pl-2 pr-2 caption white--text rounded-pill">{{ item.LimitedOffer }}</span>
              </div>
              <div class="d-block">
                <span class="caption black--text font-weight-bold">{{ item.OfferTimeBold }}</span> <span class="caption black--text">{{
                  item.OfferTimeLight }}</span>
              </div>
            </div>
          </v-card-text>
          <v-card-actions>
            <div class="du-card__button d-flex flex-row flex-wrap justify-space-between align-center">
              <span class="caption black--text text-decoration-underline"><a href="" class="black--text">{{ item.OfferBenefit }}</a></span>
              <v-btn outlined text class="body-2 text-capitalize pl-8 pr-8 pink--text text--darken-2 font-weight-bold">{{ item.Button }}</v-btn>
            </div>
          </v-card-actions>
        </v-card>
      </v-slide-item>
    </v-slide-group>
  </v-sheet>
</template>

<script>
  export default {
    data: () => ({
      items: [
        {
          YouPay: 'You Pay',
          Price: 'AED 125',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 125',
          Data: '4 GB',
          DataTitle: 'National data',
          Minutes: '100',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '4 GB free data on WiFi UAE',
          BenefitThree: 'Carry over data to next month',
          BenefitFour: 'Amazon Prime on us',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 2 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
        {
          YouPay: 'You Pay',
          Price: 'AED 200',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 200',
          Data: '26 GB',
          DataTitle: 'National data',
          Minutes: '400',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '15 GB free data on WiFi UAE',
          BenefitThree: 'Carry over data to next month',
          BenefitFour: 'Amazon Prime on us',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 2 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
        {
          YouPay: 'You Pay',
          Price: 'AED 300',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 300',
          Data: '50 GB',
          DataTitle: 'National data',
          Minutes: '1020',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '25 GB free data on WiFi UAE',
          BenefitThree: 'Carry over data to next month',
          BenefitFour: 'Amazon Prime on us',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 2 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
        {
          YouPay: 'You Pay',
          Price: 'AED 500',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 500',
          Data: '100 GB',
          DataTitle: 'National data',
          Minutes: '1500',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '100 GB free data on WiFi UAE',
          BenefitThree: 'Carry over data to next month',
          BenefitFour: 'Amazon Prime on us',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 2 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
        {
          YouPay: 'You Pay',
          Price: 'AED 1000',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 1000',
          Data: 'Unlimited',
          DataTitle: 'National data',
          Minutes: 'Unlimited',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '120 GB free data on WiFi UAE',
          BenefitThree: 'Amazon Prime on us',
          BenefitFour: 'Carry over data to next month',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 5 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
        {
          YouPay: 'You Pay',
          Price: 'AED 125',
          PerMonth: '/month',
          Months: 'For 12 months + 5% VAT',
          SubTitle: 'You Get',
          Title: 'Power Plan 125',
          Data: '4 GB',
          DataTitle: 'National data',
          Minutes: '100',
          MinutesTitle: 'Flexi minutes',
          BenefitOne: 'No activation fee. Save AED 125',
          BenefitTwo: '4 GB free data on WiFi UAE',
          BenefitThree: 'Carry over data to next month',
          BenefitFour: 'Amazon Prime on us',
          BenefitFive: 'Free Internet Calling Pack',
          BenefitSix: 'Roaming 2 GB',
          LimitedOffer: 'Limited time offer',
          OfferTimeBold: 'The Entertainer',
          OfferTimeLight: 'on us for 12 months',
          OfferBenefit: 'What you get',
          Button: 'Select',
        },
      ],
      model: null,
    }),
  };
</script>

<style>
  @import "../styles/main.css";
</style>