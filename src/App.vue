<template>
  <v-app id="inspire">
    <v-navigation-drawer
      :expand-on-hover="$vuetify.breakpoint.mdAndUp"
      :clipped="$vuetify.breakpoint.mdAndUp"
      app
      v-model="drawer"
      mini-variant-width="70"
    >
      <v-list dense nav rounded>
        <v-list-item>
          <v-list-item-avatar horizontal height="auto" class="mx-auto">
            <v-img
              src="https://img.icons8.com/emoji/48/000000/package-.png"
            ></v-img>
          </v-list-item-avatar>
          <v-list-item-title class="body-2 ml-4">Paqueteria</v-list-item-title>
        </v-list-item>
        <v-divider dark light class="mb-1"></v-divider>

        <template>
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title> Inicio </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <span style="color: grey">
                  <i class="far fa-newspaper"></i>
                </span>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 1 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <span style="color: green">
                  <i class="fas fa-chart-bar"></i>
                </span>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 2 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </template>

        <template>
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title> Admin </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-database"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 1 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-file-download"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 2 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </template>

        <template>
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title> Registro </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-search"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 1 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-table"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 2 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </template>

        <v-divider class="mb-1"></v-divider>

        <template>
          <v-list-group>
            <v-list-item slot="activator">
              <v-list-item-content>
                <v-list-item-title> Otros </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-mobile-alt" />
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 1 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-list-ul"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 2 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>

            <v-list-item :to="{ name: 'Home' }">
              <v-list-item-action>
                <i class="fas fa-user-check"></i>
              </v-list-item-action>
              <v-list-item-content>
                <v-list-item-title> Sub Pagina 3 </v-list-item-title>
              </v-list-item-content>
            </v-list-item>
          </v-list-group>
        </template>

        <v-list-item :to="{ name: 'Home' }">
          <v-list-item-action>
            <i class="fas fa-map-marked-alt"></i>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title> Pagina 1 </v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item :to="{ name: 'Home' }">
          <v-list-item-action>
            <i class="fas fa-users-cog"></i>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title> Pagina 2 </v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item :to="{ name: 'Home' }">
          <v-list-item-action>
            <i class="far fa-handshake"></i>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title> Pagina 3 </v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      :clipped-left="$vuetify.breakpoint.mdAndUp"
      src="https://picsum.photos/id/387/3072/2048"
      dark
      app
      dense
    >
      <v-toolbar-title style="width: 300px" class="ml-0 pl-4">
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
        <span>Paqueteria</span>
      </v-toolbar-title>
      <v-spacer></v-spacer>

      <v-tooltip bottom>
        <template v-slot:activator="{ on, attrs }">
          <v-btn icon v-bind="attrs" v-on="on">
            <i class="fas fa-sign-out-alt fa-2x"></i>
          </v-btn>
        </template>
        <span>Salir</span>
      </v-tooltip>
      
    </v-app-bar>

    <v-content class="pt-12">
      <v-container fluid class="fill-height">
        <v-slide-y-transition mode="out-in">
          <router-view />
        </v-slide-y-transition>
      </v-container>
    </v-content>

    <v-footer height="auto" padless>
      <v-layout justify-center>
        <v-flex text-right>
          <v-card flat tile dark class="color">
            <v-card-text class="black--text">
              Sistema &copy;{{ new Date().getFullYear() }}
            </v-card-text>
          </v-card>
        </v-flex>
      </v-layout>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: "App",

  data: () => ({
    drawer: true,
    mini: false,
  }),
};
</script>
<style>
.color {
  background: #00d2ff;
  background: -webkit-linear-gradient(to right, #3a7bd5, #00d2ff);
  background: linear-gradient(to right, #3a7bd5, #00d2ff);
}
</style>