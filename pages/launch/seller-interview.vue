<template>
  <div>
<div data-ng-controller="in-ssr-header-controller" data-ng-init="init('Header_BC_a1r2j3u4-n5s6-b7h8-a9r0-a1d2w3a4j567')" class="ng-scope">
    
        
  
<div class="a-section" style="margin:0!important">
    <div class="a-box a-box-normal a-color-offset-background"><div class="a-box-inner a-padding-base">
        <a data-ng-href="" class="a-link-normal" href="#">
            <img class="header-logo" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/sc-unified._V360962423_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/sc-unified._V360962423_.png">
        </a>
        <ul data-ng-mouseout="offFocus()" data-ng-mouseover="onFocus('settings')" class="a-unordered-list a-nostyle a-vertical header-settings-tab">
           <a class="a-link-normal ng-binding" href="/gp/sign-in/logout.html">Logout</a>
      
        </ul>
    </div></div>
</div>
            
        
    
</div>


<div class="a-box a-box-normal page-nav"><div class="a-box-inner a-padding-base">
<div class="stepRow">
    <!-- ngRepeat: step in navigation.Steps --><div ng-class="['step', getStepClass(step.currentStep ,step.stepCompletionStatus)]" ng-repeat="step in navigation.Steps" class="ng-scope step stepCompleted">

 
      <div data-ng-hide="isLinkAllowed(step)" class="stepLinkBox" title="Phone Verification">
        <img class="stepImg" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png">
        <span class="step-text ng-binding">Phone Verification</span>
      </div>

    </div><!-- end ngRepeat: step in navigation.Steps --><div ng-class="['step', getStepClass(step.currentStep ,step.stepCompletionStatus)]" ng-repeat="step in navigation.Steps" class="ng-scope step stepCompleted">



      <div data-ng-hide="isLinkAllowed(step)" class="stepLinkBox" title="Seller Information">
        <img class="stepImg" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png">
        <span class="step-text ng-binding">Seller Information</span>
      </div>

    </div><!-- end ngRepeat: step in navigation.Steps --><div ng-class="['step', getStepClass(step.currentStep ,step.stepCompletionStatus)]" ng-repeat="step in navigation.Steps" class="ng-scope step stepCompleted">

 
     <div data-ng-hide="isLinkAllowed(step)" class="stepLinkBox" title="Seller Information">
        <img class="stepImg" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/completedStepA._CB295853638_.png">
        <span class="step-text ng-binding">Tax Details</span>
      </div>

    </div><!-- end ngRepeat: step in navigation.Steps --><div ng-class="['step', getStepClass(step.currentStep ,step.stepCompletionStatus)]" ng-repeat="step in navigation.Steps" class="ng-scope step stepActive">

       <div data-ng-hide="isLinkAllowed(step)" class="stepLinkBox" title="Tax Details">
        <img class="stepImg" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/currentStepA._CB295853638_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/currentStepA._CB295853638_.png">
        <span class="step-text ng-binding">Seller Interview</span>
      </div>

    </div><!-- end ngRepeat: step in navigation.Steps --><div ng-class="['step', getStepClass(step.currentStep ,step.stepCompletionStatus)]" ng-repeat="step in navigation.Steps" class="ng-scope step stepReady">


      <div data-ng-hide="isLinkAllowed(step)" class="stepLinkBox ng-hide" title="Dashboard">
        <img class="stepImg" ng-src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/notReadyStep._CB295853632_.png" src="https://images-eu.ssl-images-amazon.com/images/G/31/rainier/nav/notReadyStep._CB295853632_.png">
        <span class="step-text ng-binding">Dashboard</span>
      </div>

    </div><!-- end ngRepeat: step in navigation.Steps -->
  </div>
</div></div>

    <div class="a-section main container section">
      <div class="a-section a-spacing-none">
        <h2
          class="a-spacing-small a-color-state page-step-heading a-text-normal"
        >Choose categories you wish to sell</h2>
      </div>

      <div class="a-section a-spacing-base a-spacing-top-base">
        <div
          data-ng-controller="seller-interview-category-controller"
          data-ng-init="init('Seller_Interview_Category_BC_67635828-f378-41af-bc81-b6c1b3b8b032')"
          class="a-section interview-fragment ng-scope"
        >
          <div class="a-section a-spacing-none">
            <span
              class="a-size-base-plus a-color-tertiary ng-binding"
            >Choose categories you wish to sell</span>
          </div>

          <!-- ngRepeat: categoryGroup in categoryList -->
          <div
             v-for="p in interview_data" :key="p.id"
            class="a-section a-spacing-mini category-group ng-scope"
          >
            <span
              class="a-size-base a-color-secondary a-text-bold ng-binding"
            >{{p.name}}</span>

            <!-- ngRepeat: category in categoryGroup.categories -->
            <span v-for="q in p.data" :key="q.id" class="ng-scope">
              <div class="a-checkbox a-checkbox-fancy checkbox-text a-spacing-top-mini ng-scope">
                <label>
                  <input
                    type="checkbox"
                    name="categoryCheckbox"
                    value="gl_book"
                    data-a-input-name="categoryCheckbox"
                    data-ng-model="categoryModel[category.id]"
                    data-ng-true-value
                    class="ng-pristine ng-valid"
                  />
                  <i class="a-icon a-icon-checkbox"></i>
                  <span class="a-label a-checkbox-label ng-binding">{{q.name}}</span>
                </label>
              </div>
            </span>
           
          </div>
          <!-- end ngRepeat: categoryGroup in categoryList -->

          <div data-ng-show="showError" class="a-section a-spacing-base ng-hide">
            <div
              class="a-box a-alert-inline a-alert-inline-error"
              aria-live="assertive"
              role="alert"
            >
              <div class="a-box-inner a-alert-container">
                <i class="a-icon a-icon-alert"></i>
                <div class="a-alert-content ng-binding">Please choose any one of the option</div>
              </div>
            </div>
          </div>
          <hr class="a-divider-normal" />
        </div>
      </div>

      <div class="a-section a-spacing-base a-spacing-top-base">
        <div
          data-ng-controller="seller-interview-checkbox-controller"
          data-ng-init="init('Seller_Interview_Seller_Info_BC_67635828-f378-41af-bc81-b6c1b3b8b032')"
          class="a-section interview-fragment ng-scope"
        >
          <!-- ngRepeat: (key, value) in sellerInterviewConfig -->
          <div
            id="sellerInfo"
            data-ng-repeat="(key, value) in sellerInterviewConfig"
            class="a-section a-spacing-none checkbox-question-container ng-scope"
          >
            <p
              class="a-spacing-top-small a-size-base a-color-secondary a-text-bold ng-binding"
            >Where do you get products from?</p>

            <!-- ngRepeat: option in renderOptions[key] -->
            <span data-ng-repeat="option in renderOptions[key]" class="ng-scope">
              <div
                class="a-checkbox a-checkbox-fancy category-checkbox-text a-spacing-top-mini ng-scope"
              >
                <label>
                  <input
                    type="checkbox"
                    name
                    value="manufacturer"
                    data-a-input-name
                    data-ng-model="checkboxModel[value.renderConfig.id][option.id]"
                    class="ng-pristine ng-valid"
                  />
                  <i class="a-icon a-icon-checkbox"></i>
                  <span class="a-label a-checkbox-label ng-binding">I manufacture them</span>
                </label>
              </div>
            </span>
            <!-- end ngRepeat: option in renderOptions[key] -->
            <span data-ng-repeat="option in renderOptions[key]" class="ng-scope">
              <div
                class="a-checkbox a-checkbox-fancy category-checkbox-text a-spacing-top-mini ng-scope"
              >
                <label>
                  <input
                    type="checkbox"
                    name
                    value="reseller"
                    data-a-input-name
                    data-ng-model="checkboxModel[value.renderConfig.id][option.id]"
                    class="ng-pristine ng-valid"
                  />
                  <i class="a-icon a-icon-checkbox"></i>
                  <span class="a-label a-checkbox-label ng-binding">I resell product that I buy</span>
                </label>
              </div>
            </span>
            <!-- end ngRepeat: option in renderOptions[key] -->
            <span data-ng-repeat="option in renderOptions[key]" class="ng-scope">
              <div
                class="a-checkbox a-checkbox-fancy category-checkbox-text a-spacing-top-mini ng-scope"
              >
                <label>
                  <input
                    type="checkbox"
                    name
                    value="importer"
                    data-a-input-name
                    data-ng-model="checkboxModel[value.renderConfig.id][option.id]"
                    class="ng-pristine ng-valid"
                  />
                  <i class="a-icon a-icon-checkbox"></i>
                  <span class="a-label a-checkbox-label ng-binding">I import them</span>
                </label>
              </div>
            </span>
            <!-- end ngRepeat: option in renderOptions[key] -->

            <div
              data-ng-show="sellerInfo"
              class="a-section a-spacing-none a-spacing-top-small ng-hide"
            >
              <div
                class="a-box a-alert-inline a-alert-inline-error"
                aria-live="assertive"
                role="alert"
              >
                <div class="a-box-inner a-alert-container">
                  <i class="a-icon a-icon-alert"></i>
                  <div class="a-alert-content ng-binding">Please choose any one of the option</div>
                </div>
              </div>
            </div>
          </div>
          <!-- end ngRepeat: (key, value) in sellerInterviewConfig -->
          <hr class="a-spacing-base a-spacing-top-base a-divider-normal" />
        </div>
      </div>


      <div class="a-section a-spacing-base a-spacing-top-base">
        <div
          data-ng-controller="seller-interview-dropdown-controller"
          data-ng-init="init('Seller_Interview_Dropdown_BC_67635828-f378-41af-bc81-b6c1b3b8b032')"
          class="a-section interview-fragment ng-scope"
        >
          <!-- ngRepeat: (key, value) in sellerInterviewConfig -->
          <div
            data-ng-repeat="(key, value) in sellerInterviewConfig"
            class="a-section a-spacing-base dropdown-question-container ng-scope"
          >
            <p
              class="a-size-base a-color-secondary a-text-bold ng-binding"
            >What is your annual turnover ?</p>
            <span class="a-dropdown-container">
              <select
                name="product-quantity-dropdown"
                autocomplete="off"
                data-a-native-class="dropdown-question"
                id="sellerTurnoverInfo"
                tabindex="-1"
                class="a-native-dropdown dropdown-question"
              >
                <option class="a-prompt ng-binding" value>Select an option</option>
                <!-- ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="mini"
                  class="ng-scope ng-binding"
                >Rs 1 - 500</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="small"
                  class="ng-scope ng-binding"
                >Rs 501 - 1000</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="medium"
                  class="ng-scope ng-binding"
                >Rs 1001 - 5000</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="large"
                  class="ng-scope ng-binding"
                >Rs 5001 - 20000</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="extra_large"
                  class="ng-scope ng-binding"
                >Higher than Rs 20000</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
              </select>
            </span>

            <div data-ng-show="sellerTurnoverInfo" class="a-section a-spacing-top-mini ng-hide">
              <div
                class="a-box a-alert-inline a-alert-inline-error"
                aria-live="assertive"
                role="alert"
              >
                <div class="a-box-inner a-alert-container">
                  <i class="a-icon a-icon-alert"></i>
                  <div class="a-alert-content ng-binding">Please choose any one of the option</div>
                </div>
              </div>
            </div>
          </div>
          <!-- end ngRepeat: (key, value) in sellerInterviewConfig -->
          <div
            data-ng-repeat="(key, value) in sellerInterviewConfig"
            class="a-section a-spacing-base dropdown-question-container ng-scope"
          >
            <p
              class="a-size-base a-color-secondary a-text-bold ng-binding"
            >How many products do you sell ?</p>
            <span class="a-dropdown-container">
              <select
                name="product-quantity-dropdown"
                autocomplete="off"
                data-a-native-class="dropdown-question"
                id="sellerProductQuantity"
                tabindex="-1"
                class="a-native-dropdown dropdown-question"
              >
                <option class="a-prompt ng-binding" value>Select an option</option>
                <!-- ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="mini"
                  class="ng-scope ng-binding"
                >0 - 5</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="small"
                  class="ng-scope ng-binding"
                >6 - 20</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="medium"
                  class="ng-scope ng-binding"
                >21 - 50</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="large"
                  class="ng-scope ng-binding"
                >51 - 500</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
                <option
                  data-ng-click="changeOption(option.id)"
                  data-ng-repeat="option in renderOptions[key]"
                  value="extra_large"
                  class="ng-scope ng-binding"
                >Greater than 500</option>
                <!-- end ngRepeat: option in renderOptions[key] -->
              </select>
            </span>

            <div data-ng-show="sellerProductQuantity" class="a-section a-spacing-top-mini ng-hide">
              <div
                class="a-box a-alert-inline a-alert-inline-error"
                aria-live="assertive"
                role="alert"
              >
                <div class="a-box-inner a-alert-container">
                  <i class="a-icon a-icon-alert"></i>
                  <div class="a-alert-content ng-binding">Please choose any one of the option</div>
                </div>
              </div>
            </div>
          </div>
          <!-- end ngRepeat: (key, value) in sellerInterviewConfig -->
          <hr class="a-spacing-base a-divider-normal" />
        </div>
      </div>

      <div class="a-section a-spacing-base a-spacing-top-base">
        <div
          data-ng-controller="seller-interview-radio-controller"
          data-ng-init="init('Seller_Interview_Other_Platform_BC_67635828-f378-41af-bc81-b6c1b3b8b032')"
          class="a-section interview-fragment ng-scope"
        >
          <input type="hidden" name data-ng-init="isBrowser = true" />

          <!-- ngRepeat: (key, value) in sellerInterviewConfig -->
          <div
            data-ng-repeat="(key, value) in sellerInterviewConfig"
            class="a-section a-spacing-none radio-question-container ng-scope"
          >
            <p
              class="a-spacing-top-small a-size-base a-color-secondary a-text-bold ng-binding"
            >Do you sell in other websites ?</p>

            <fieldset class="a-spacing-small a-form-horizontal">
              <!-- ngRepeat: option in renderOptions[key] -->
              <span data-ng-repeat="option in renderOptions[key]" class="radio-option ng-scope">
                <div class="a-radio a-radio-fancy ng-scope">
                  <label for="yes">
                    <input
                      id="yes"
                      type="radio"
                      name="sellerOtherPlatformInfo"
                      value="yes"
                      data-a-input-name="sellerOtherPlatformInfo"
                      data-ng-model="radioButtonModel[value.renderConfig.id]"
                      class="ng-pristine ng-valid"
                    />
                    <i class="a-icon a-icon-radio"></i>
                    <span class="a-label a-radio-label ng-binding">Yes</span>
                  </label>
                </div>
              </span>
              <!-- end ngRepeat: option in renderOptions[key] -->
              <span data-ng-repeat="option in renderOptions[key]" class="radio-option ng-scope">
                <div class="a-radio a-radio-fancy ng-scope">
                  <label for="no">
                    <input
                      id="no"
                      type="radio"
                      name="sellerOtherPlatformInfo"
                      value="no"
                      data-a-input-name="sellerOtherPlatformInfo"
                      data-ng-model="radioButtonModel[value.renderConfig.id]"
                      class="ng-pristine ng-valid"
                    />
                    <i class="a-icon a-icon-radio"></i>
                    <span class="a-label a-radio-label ng-binding">No</span>
                  </label>
                </div>
              </span>
              <!-- end ngRepeat: option in renderOptions[key] -->
            </fieldset>

            <div data-ng-show="sellerOtherPlatformInfo" class="a-section a-spacing-mini ng-hide">
              <div
                class="a-box a-alert-inline a-alert-inline-error"
                aria-live="assertive"
                role="alert"
              >
                <div class="a-box-inner a-alert-container">
                  <i class="a-icon a-icon-alert"></i>
                  <div class="a-alert-content ng-binding">Please choose any one of the option</div>
                </div>
              </div>
            </div>
            <!-- ngIf: value.renderConfig.showDivider === 'true' -->
          </div>
          <!-- end ngRepeat: (key, value) in sellerInterviewConfig -->
        </div>
      </div>

     
      <div class="a-section a-spacing-base a-spacing-top-base">
        <div
          data-ng-controller="seller-interview-input-controller"
          data-ng-init="init('Seller_Interview_Product_Link_BC_67635828-f378-41af-bc81-b6c1b3b8b032')"
          class="a-section interview-fragment ng-scope"
        >
          <!-- ngRepeat: (key, value) in sellerInterviewConfig -->
          <div
            data-ng-repeat="(key, value) in sellerInterviewConfig"
            class="a-section a-spacing-small ng-scope"
          >
            <div class="a-section a-spacing-none text-input-container" style="display: none;">
              <input
                type="url"
                placeholder="Paste url of any product on the website"
                name="productURL"
                class="a-input-text interview-text-input ng-scope ng-pristine ng-valid ng-valid-url"
                data-ng-keyup="textChanged(links[value.renderConfig.id])"
                data-ng-model="links[value.renderConfig.id]"
              />

              <div
                data-ng-show="productURL"
                class="a-section a-spacing-none a-spacing-top-small ng-hide"
              >
                <div
                  class="a-box a-alert-inline a-alert-inline-error"
                  aria-live="assertive"
                  role="alert"
                >
                  <div class="a-box-inner a-alert-container">
                    <i class="a-icon a-icon-alert"></i>
                    <div class="a-alert-content ng-binding">Please provide a valid product url</div>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <!-- end ngRepeat: (key, value) in sellerInterviewConfig -->
          <hr class="a-spacing-top-large a-divider-normal" />
        </div>
      </div>

      <span class="a-button a-spacing-top-medium a-button-primary final-submit" id="a-autoid-2">
        <span class="a-button-inner">
          <input
            data-ng-click="submit()"
            class="a-button-input"
            type="submit"
            aria-labelledby="a-autoid-2-announce"
          />
          <span class="a-button-text" aria-hidden="true" id="a-autoid-2-announce">Next</span>
        </span>
      </span>
    </div>

    <Aside class="container"/>
  </div>
</template>

<script>


import Aside from '@/components/aside'

export default {

data(){
    return{
        interview_data: [
        {
          id: 1,
          name: 'Books, Movies & Games',
          data: [
            {
              id: 1,
              name: 'Books'
            },
            {
              id: 2,
              name: 'Movies'
            },
            {
              id: 3,
              name: 'Muscial Instruments'
            },
            {
              id: 4,
              name: 'Music'
            },
            {
              id: 5,
              name: 'Video Games'
            }
          ]
        },
        {
          id: 2,
          name: 'Clothing, Shoes & Jewelry',
          data: [
            {
              id: 1,
              name: 'Clothing'
            },
            {
              id: 2,
              name: 'Shoes'
            },
            {
              id: 3,
              name: 'Watches'
            },
            {
              id: 4,
              name: 'Jewelery'
            },
            {
              id: 5,
              name: 'Luggage'
            }
          ]
        },
        {
          id: 3,
          name: 'Home, Garden & Tools, Furniture',
          data: [
            {
              id: 1,
              name: 'Home'
            },
            {
              id: 2,
              name: 'Large Appliances'
            },
            {
              id: 3,
              name: 'Pet Supplies'
            },
            {
              id: 4,
              name: 'Kitchen'
            },
            {
              id: 5,
              name: 'Furniture'
            }
          ]
        },
        {
          id: 4,
          name: 'Beauty, Health & Grocceries',
          data: [
            {
              id: 1,
              name: 'Beauty'
            },
            {
              id: 2,
              name: 'Grocery'
            },
            {
              id: 3,
              name: 'Health'
            },
            {
              id: 4,
              name: 'Personal Care Appliances'
            }
          ]
        },
        {
          id: 5,
          name: 'Electronics & Computers',
          data: [
            {
              id: 1,
              name: 'Consumer Electronics'
            },
            {
              id: 2,
              name: 'Mobile Phones'
            },
            {
              id: 3,
              name: 'Personal Computers'
            },
            {
              id: 4,
              name: 'Office Products'
            },
            {
              id: 5,
              name: 'Software'
            }
          ]
        },
        {
          id: 6,
          name: 'Toys & Baby, Sports',
          data: [
            {
              id: 1,
              name: 'Baby'
            },
            {
              id: 2,
              name: 'Toys'
            },
            {
              id: 3,
              name: 'Sporting Goods'
            }
          ]
        },        {
          id: 7,
          name: 'Automotive and Industrial Suppy',
          data: [
            {
              id: 1,
              name: 'Automotive'
            },
            {
              id: 2,
              name: 'Industrial Supply'
            }
          ]
        },
        {
          id: 8,
          name: 'Other',
          data: [
            {
              id: 1,
              name: 'My Category is not listed here'
            }
          ]
        }
      ]
    }
},

          components:{
    Aside
  },
}
</script>


<style scoped>
.a-section:last-child{
    margin-bottom: 20px!important
}
</style>