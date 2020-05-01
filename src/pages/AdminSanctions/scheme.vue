<template>
  <form>
    <md-card>
      <md-card-header data-background-color="green">
        <h4 class="title">Scheme details</h4>
        <p class="category">Provide Scheme details as per AS Letter</p>
      </md-card-header>

      <md-card-content>
        <div class="md-layout"> 
            <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>Select Organisation</label>


              <!-- v-for loop for organisation-->
              <md-select v-model="country" name="country" id="country" placeholder="organisation">
                <md-option value="australia">Australia</md-option>
                <md-option value="brazil">Brazil</md-option>
                <md-option value="japan">Japan</md-option>
                <md-option value="united-states">United States</md-option>
              </md-select>
            </md-field>
          </div>         


          <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>Create Scheme id   (Eg:NSP,MOP)</label>
              <md-input v-model="schemeid" type="text"></md-input>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>Create Respective Year of AS (in format yy-yy(18-19))</label>
              <md-input v-model="year" type="text"></md-input>
            </md-field>
          </div>
          <div class="md-layout-item md-small-size-100 md-size-50">
            <md-field>
              <label>Scheme Name</label>
              <md-input v-model="schemename" type="text">{{ }}</md-input>
            </md-field>
          </div>
                 
          <div class="md-layout-item md-size-100">
            <md-field maxlength="5">
              <label>About Scheme</label>
              <md-textarea v-model="aboutme"></md-textarea>
            </md-field>
          </div>
          <div class="md-layout-item md-size-100 text-right">
            <md-button class="md-raised md-success">Submit</md-button>
          </div>
        </div>
      </md-card-content>
    </md-card>
  </form>
</template>
<script>
export default {
  name: "scheme",
  props: {
    dataBackgroundColor: {
      type: String,
      default: ""
    }
  },
  data() {
    return {
      usernOrganisation: null,
      schemeid: null,
      years: null,
      schemename: null,
      address: null,
      city: null,
      country: null,
      code: null,
      aboutme:
        " "
    };

  }
};
</script>
<style></style>



