<template>
  <div>
    <v-app-bar color="white" dark>
      <v-spacer></v-spacer>
      <v-toolbar-title class="primary--text font-weight-bold display-1"
        >Universal Payment system</v-toolbar-title
      >
      <v-spacer></v-spacer>

      <v-menu left bottom offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on" color="primary">
            <v-icon>mdi-dots-vertical</v-icon>
          </v-btn>
        </template>

        <v-list>
          <v-list-item
            v-for="list in lists"
            :key="list.title"
            @click="() => {}"
          >
            <!-- <v-list-item-title>Option {{ n }}</v-list-item-title> -->
            <v-list-item-title class="mx-5 my-2">
              <v-icon left flat>{{ list.icon }}</v-icon
              ><span>{{ list.title }}</span>
            </v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </v-app-bar>
    <!---->
    <v-navigation-drawer app color="primary">
      <v-list-item>
        <v-list-item-content>
          <div class="align-center justify-center">
            <v-avatar size="100">
              <img src="../assets/images/logo.jpeg" alt="John" />
            </v-avatar>
          </div>
          <v-list-item-title class="text-h6 text-weight-bold white--text"
            >Universal payment</v-list-item-title
          >
          <v-list-item-subtitle></v-list-item-subtitle>
        </v-list-item-content>
      </v-list-item>

      <v-divider></v-divider>

      <!-- <v-list >
        <v-list-item >
          <v-list-item-icon>
            <v-icon></v-icon>
          </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list> -->
      <v-list>
        <v-list-item v-for="item in items" :key="item.title" link>
            <v-list-item-icon>
                    <v-icon dark>{{item.icon}}</v-icon>
            </v-list-item-icon>
            <v-list-item-content>
                <v-list-item-title>
                        {{item.title}}
                </v-list-item-title>
            </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  name: "Navtop",
  data: () => ({
    lists: [
      { icon: "mdi-account", title: "profile", link: "/profile" },
      { icon: "mdi-account", title: "profile", link: "/profile" },
      { icon: "mdi-account", title: "profile", link: "/profile" },
      { icon: "mdi-logout", title: "logout", link: "/logout" },
    ],
    items: [
      { title: "Dashboard", icon: "mdi-view-dashboard" },
      { title: "Photos", icon: "mdi-image" },
      { title: "About", icon: "mdi-help-box" },
    ],
  }),
};
</script>

<style>
</style>