<template>
  <div class="home">
    <v-list subheader two-line flat>

      <v-list-item-group v-model="settings" multiple>
        <v-list-item>
          <template v-slot:default="{ active }">
            <v-list-item-action>
              <v-checkbox :input-value="active" color="primary"></v-checkbox>
            </v-list-item-action>

            <v-list-item-content>
              <v-list-item-title>Wake Up</v-list-item-title>
            </v-list-item-content>
          </template>
        </v-list-item>

      </v-list-item-group>
    </v-list>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
