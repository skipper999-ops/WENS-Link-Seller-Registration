<template>
  <div>
    <div id="a-page">
      <div class="a-section a-padding-medium auth-workflow">
        <div class="a-section a-spacing-none auth-navbar">
          <div class="a-section a-spacing-medium a-text-center">
            <img src />
          </div>
        </div>

        <div id="authportal-center-section" class="a-section">
          <div id="authportal-main-section" class="a-section">

            <div class="a-section auth-pagelet-container">

              <!-- show a warning modal dialog when the third party account is connected with WENS Link -->

              <div class="a-section auth-pagelet-container">
                <form
                  id="ap_register_form"
                  name="register"
                  method="post"
                  novalidate
                  action="https://sellercentral.WENS Link.in/ap/register"
                  class="ap_ango_default auth-validate-form-moa fwcim-form"
                  data-fwcim-id="078d6cd3"
                >

                  <div class="a-box a-spacing-extra-large">
                    <div class="a-box-inner">
                      <h1 class="a-spacing-small moa_desktop_signup">Create Account</h1>

                      <div class="a-row a-spacing-base">
                        <label for="ap_customer_name" class="a-form-label">Your name</label>

                        <input
                          type="text"
                          maxlength="50"
                          id="ap_customer_name"
                          autocomplete="off"
                          name="customerName"
                          tabindex="1"
                          class="a-input-text a-span12 auth-autofocus auth-required-field"
                        />

                        <div
                          id="auth-customerName-missing-alert"
                          class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                          aria-live="assertive"
                          role="alert"
                        >
                          <div class="a-box-inner a-alert-container">
                            <i class="a-icon a-icon-alert"></i>
                            <div class="a-alert-content">Enter your name</div>
                          </div>
                        </div>
                      </div>

                      <div class="a-section a-spacing-base ap_mobile_number_fields">
                        <div class="a-row">
                          <label
                            for="ap_phone_number"
                            class="a-form-label auth-mobile-label"
                          >Mobile number</label>

                          <div class="a-fixed-left-grid a-spacing-top-mini">
                            <div class="a-fixed-left-grid-inner" style="padding-left:85px">
                              <div
                                class="a-fixed-left-grid-col a-col-left"
                                style="width:85px;margin-left:-85px;float:left;"
                              >
                                <span class="a-dropdown-container">
                                  <select
                                    name="countryCode"
                                    style="display: none;"
                                    autocomplete="off"
                                    data-a-touch-header="Country/Region Code"
                                    id="auth-country-picker"
                                    tabindex="-1"
                                    class="a-native-dropdown"
                                  >
                                    <option
                                      data-calling-code="91"
                                      data-country-code="IN"
                                      value="IN"
                                      data-a-html-content="India +91"
                                      selected
                                    >IN +91</option>
                                  </select>
                                  <span
                                    tabindex="-1"
                                    id="auth-country-picker-container"
                                    class="a-button a-button-dropdown"
                                    style="min-width: 0.403587%;"
                                  >
                                    <span class="a-button-inner">
                                      <span
                                        class="a-button-text a-declarative"
                                        data-action="a-dropdown-button"
                                        role="button"
                                        tabindex="0"
                                        aria-hidden="true"
                                      >
                                        <span class="a-dropdown-prompt">IN +91</span>
                                      </span>
                                      <i class="a-icon a-icon-dropdown"></i>
                                    </span>
                                  </span>
                                </span>
                              </div>
                              <div
                                class="a-fixed-left-grid-col a-col-right"
                                style="padding-left:2%;float:left;"
                              >
                                <input
                                  type="tel"
                                  maxlength="50"
                                  id="ap_phone_number"
                                  placeholder="Mobile number"
                                  name="email"
                                  tabindex="3"
                                  class="a-input-text a-span12 a-spacing-micro auth-required-field auth-require-phone-validation"
                                  data-validation-id="phoneNumber"
                                />

                                <div
                                  id="auth-phoneNumber-missing-alert"
                                  class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                                  aria-live="assertive"
                                  role="alert"
                                >
                                  <div class="a-box-inner a-alert-container">
                                    <i class="a-icon a-icon-alert"></i>
                                    <div class="a-alert-content">Enter your mobile number</div>
                                  </div>
                                </div>

                                <div
                                  id="auth-phoneNumber-invalid-phone-alert"
                                  class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                                  aria-live="assertive"
                                  role="alert"
                                >
                                  <div class="a-box-inner a-alert-container">
                                    <i class="a-icon a-icon-alert"></i>
                                    <div
                                      class="a-alert-content"
                                    >The mobile number you entered does not seem to be valid</div>
                                  </div>
                                </div>

                                <div
                                  id="auth-email-missing-alert-ango-phone"
                                  class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                                  aria-live="assertive"
                                  role="alert"
                                >
                                  <div class="a-box-inner a-alert-container">
                                    <i class="a-icon a-icon-alert"></i>
                                    <div class="a-alert-content">Enter your mobile number</div>
                                  </div>
                                </div>
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>

                      <div class="a-section a-spacing-base ap_email_fields">
                        <div class="a-row a-spacing-micro">
                          <label for="ap_email" class="a-form-label">Email (optional)</label>
                          <input
                            type="email"
                            maxlength="64"
                            id="ap_email"
                            name="secondaryLoginClaim"
                            tabindex="4"
                            class="a-input-text a-span12 auth-require-email-validaton"
                            data-validation-id="email"
                          />

                          <div
                            id="auth-email-missing-alert"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Enter your email</div>
                            </div>
                          </div>

                          <div
                            id="auth-email-invalid-email-alert"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Enter a valid email address</div>
                            </div>
                          </div>

                          <div
                            id="auth-email-invalid-claim-alert"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div
                                class="a-alert-content"
                              >Wrong or Invalid email address or mobile phone number. Please correct and try again.</div>
                            </div>
                          </div>

                          <div
                            id="auth-email-missing-alert-ango-email"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Enter your email</div>
                            </div>
                          </div>

                          <div
                            id="auth-email-missing-alert-ango-phone"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Enter your mobile phone number</div>
                            </div>
                          </div>
                        </div>
                      </div>

                      <div class="auth-require-fields-match-group">
                        <div class="a-row a-spacing-base">
                          <label for="ap_password" class="a-form-label">Password</label>

                          <input
                            type="password"
                            maxlength="1024"
                            id="ap_password"
                            autocomplete="off"
                            placeholder="At least 6 characters"
                            name="password"
                            tabindex="5"
                            class="a-input-text a-span12 auth-required-field auth-require-fields-match auth-require-password-validation"
                          />

                          <div
                            class="a-box a-alert-inline a-alert-inline-info auth-inlined-information-message a-spacing-top-mini"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Passwords must be at least 6 characters.</div>
                            </div>
                          </div>

                          <div
                            id="auth-password-missing-alert"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Enter your password</div>
                            </div>
                          </div>

                          <div
                            id="auth-password-invalid-password-alert"
                            class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                            aria-live="assertive"
                            role="alert"
                          >
                            <div class="a-box-inner a-alert-container">
                              <i class="a-icon a-icon-alert"></i>
                              <div class="a-alert-content">Passwords must be at least 6 characters.</div>
                            </div>
                          </div>
                        </div>
                      </div>

                      <div
                        class="a-section a-spacing-top-large a-text-left ap_mobile_number_fields"
                      >
                        <div class="a-row">We will send you a text to verify your phone.</div>
                        <div class="a-row">Message and Data rates may apply.</div>
                      </div>

                      <div class="a-section a-spacing-extra-large ap_mobile_number_fields">
                        <span
                          id="auth-continue"
                          class="a-button a-button-span12 a-button-primary auth-requires-verify-modal"
                        >
                          <span class="a-button-inner">
                            <span @click="createAccount"
                              id="auth-continue-announce"
                              class="a-button-text"
                              aria-hidden="true"
                            >Continue</span>
                          </span>
                        </span>
                      </div>

                      <div class="a-divider a-divider-section">
                        <div class="a-divider-inner"></div>
                      </div>

                      <div class="a-row">
                        Already have an account?
                        <nuxt-link to="/login">Sign In</nuxt-link>
                      </div>
                    </div>
                  </div>
                </form>
              </div>
            </div>
          </div>
        </div>

        <div id="right-2"></div>

        <div class="a-section a-spacing-top-extra-large auth-footer">
          <div class="a-divider a-divider-section">
            <div class="a-divider-inner"></div>
          </div>

          <div class="a-section a-spacing-small a-text-center a-size-mini">
            <span class="auth-footer-seperator"></span>
          </div>

          <div class="a-section a-spacing-none a-text-center">
            <span
              class="a-size-mini a-color-secondary"
            >© 1996-2019, WENS Link.com, Inc. or its affiliates</span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>


<script>


import axios from 'axios'


export default {
  methods:{
    createAccount: function(){



     var payload = new FormData()

     payload.append('name', $("#ap_customer_name").val())
     payload.append('phone_number', $("#ap_phone_number").val())
     payload.append('email', $("#ap_email").val())
     payload.append('password', $("#ap_password").val())




            axios({
                method: 'POST',
                data: payload,
                url: 'http://127.0.0.1:8000/backend/api/vendors/create/',
                contentType: 'application/json',
                data: payload
            })
                .then(res => {
                    console.log(res.data)
                    console.log('response')
                    localStorage.setItem('phone' , $("#ap_phone_number").val())
                    this.$router.push('/verification')
                })
                .catch(err => {
                    console.log('error in request', err)
                })





    }
  }
}
</script>

<style scoped>
.a-alert-inline{
  display: none!important
}
</style>