<template>
  <div>
    <div id="a-page">
      <div class="a-section a-padding-medium auth-workflow">
        <div class="a-section a-spacing-none auth-navbar">
          <div class="a-section a-spacing-medium a-text-center">
            <img
              src=""
            />
          </div>
        </div>

        <div id="authportal-center-section" class="a-section">
          <div id="authportal-main-section" class="a-section">


            <div class="a-section auth-pagelet-container">
              <!-- Set cross domain sso variables to be used for making Ajax calls to central Identity domain -->

              <!-- Set cross domain sso variables to be used for making Ajax calls to central Identity domain -->

              <!-- show a warning modal dialog when the third party account is connected with WENS Link -->

              <div class="a-section a-spacing-base">
                <div class="a-section">
                  <form
                    name="signIn"
                    method="post"
                    novalidate
                    action="https://sellercentral.WENS Link.in/ap/signin"
                    class="a-spacing-none fwcim-form"
                    data-fwcim-id="dd379249"
                  >

                    <div class="a-section">
                      <div class="a-box">
                        <div class="a-box-inner a-padding-extra-large">
                          <h1 class="a-spacing-small">Login</h1>
                          <!-- optional subheading element -->

                          <div class="a-row a-spacing-base">
                            <label for="ap_email" class="a-form-label">Email or mobile phone number</label>

                            <input
                              type="email"
                              maxlength="128"
                              id="ap_email"
                              name="email"
                              tabindex="1"
                              class="a-input-text a-span12 auth-autofocus auth-required-field"
                            />

                            <div
                              id="auth-email-missing-alert"
                              class="a-box a-alert-inline a-alert-inline-error auth-inlined-error-message a-spacing-top-mini"
                              aria-live="assertive"
                              role="alert"
                            >
                              <div class="a-box-inner a-alert-container">
                                <i class="a-icon a-icon-alert"></i>
                                <div class="a-alert-content">Enter your email or mobile phone number</div>
                              </div>
                            </div>
                          </div>

                          <input type="hidden" name="create" value="0" />

                          <div class="a-section a-spacing-large">
                            <div class="a-row">
                              <div class="a-column a-span5">
                                <label for="ap_password" class="a-form-label">Password</label>
                              </div>

                              <div class="a-column a-span7 a-text-right a-span-last">
                                <a
                                  id="auth-fpp-link-bottom"
                                  class="a-link-normal"
                                  tabindex="3"
                                  href="https://sellercentral.WENS Link.in/ap/forgotpassword?showRememberMe=true&amp;openid.identity=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier_select&amp;marketPlaceId=A21TJRUUN4KGV&amp;pageId=amzn_sw_signup_in&amp;openid.return_to=https%3A%2F%2Fsellercentral.WENS Link.in%2Fsw%2Fin%2FINSSR%2Fstep%2FSignUp%3Fpassthrough%252Faccount%3Dsoa%26passthrough%252FsuperSource%3DOAR%26ref_%3Das_in_soa_hp%26passthrough%252FmarketplaceID%3DA21TJRUUN4KGV%26passthrough%252F%26productTier%3DSILVER%26productType%3DSellOnWENS Link%26marketplaceId%3DA21TJRUUN4KGV%26passthrough%252Ftag%3DREDIRECTT1%26redirectAP%3D1&amp;prevRID=CYNRM35MQCJC1BR99Y6D&amp;openid.assoc_handle=amzn_sw_signup_in&amp;openid.mode=checkid_setup&amp;prepopulatedLoginId=&amp;failedSignInCount=0&amp;openid.claimed_id=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0%2Fidentifier_select&amp;openid.ns=http%3A%2F%2Fspecs.openid.net%2Fauth%2F2.0"
                                >Forgot Password</a>
                              </div>
                            </div>

                            <input
                              type="password"
                              maxlength="1024"
                              id="ap_password"
                              name="password"
                              tabindex="2"
                              class="a-input-text a-span12 auth-required-field"
                            />

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
                          </div>

                          <div class="a-section a-spacing-extra-large">
                            <span class="a-button a-button-span12 a-button-primary" id="a-autoid-0">
                              <span class="a-button-inner">
                                <input
                                  id="signInSubmit"
                                  tabindex="5"
                                  class="a-button-input"
                                  type="submit"
                                  aria-labelledby="a-autoid-0-announce"
                                />
                                <span
                                  class="a-button-text"
                                  aria-hidden="true"
                                  id="a-autoid-0-announce"
                                >Login</span>
                              </span>
                            </span>

                            <div id="legalTextRow" class="a-row a-spacing-top-medium a-size-small"></div>
                            <div class="a-row a-spacing-top-medium">
                              <div class="a-section a-text-left">
                                <label for="auth-remember-me" class="a-form-label">
                                  <div data-a-input-name="rememberMe" class="a-checkbox">
                                    <label>
                                      <input
                                        type="checkbox"
                                        name="rememberMe"
                                        value="true"
                                        tabindex="4"
                                      />
                                      <i class="a-icon a-icon-checkbox"></i>
                                      <span class="a-label a-checkbox-label">
                                        Keep me signed in.
                                        <span
                                          class="a-declarative"
                                          data-action="a-popover"
                                          data-a-popover="{&quot;activate&quot;:&quot;onclick&quot;,&quot;header&quot;:&quot;\&quot;Keep Me Signed In\&quot; Checkbox&quot;,&quot;inlineContent&quot;:&quot;\u003cp>Choosing \&quot;Keep me signed in\&quot; reduces the number of times you're asked to Sign-In on this device.\u003c\/p>\n\u003cp>To keep your account secure, use this option only on your personal devices.\u003c\/p>&quot;}"
                                        >
                                          <a
                                            id="remember_me_learn_more_link"
                                            href="javascript:void(0)"
                                            class="a-popover-trigger a-declarative"
                                          >
                                            Details
                                            <i class="a-icon a-icon-popover"></i>
                                          </a>
                                        </span>
                                      </span>
                                    </label>
                                  </div>
                                </label>
                              </div>
                            </div>
                          </div>

                          <div class="a-divider a-divider-break">
                            <h5>New to WENS Link?</h5>
                          </div>
                          <span
                            id="auth-create-account-link"
                            class="a-button a-button-span12 a-button-base"
                          >
                            <span class="a-button-inner">
                              <nuxt-link to="/register_account" class="a-button-text"
                              >Create your WENS Link account</nuxt-link>
                            </span>
                          </span>
                        </div>
                      </div>
                    </div>
                  </form>
                </div>
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

      <div id="auth-external-javascript" class="auth-external-javascript" data-external-javascripts></div>

      <!-- cache slot rendered -->
    </div>
  </div>
</template>