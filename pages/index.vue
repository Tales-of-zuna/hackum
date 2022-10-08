<template>
  <v-container grid-list-xs>
    <v-carousel
      hide-delimiters
      :show-arrows="false"
      class="rounded-xl my-10"
      height="300"
    >
      <v-carousel-item src="https://i.imgur.com/VTPmZCQ.png"></v-carousel-item>
    </v-carousel>
    <v-row>
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln6-2.fna.fbcdn.net/v/t1.6435-9/55837866_364808054245206_4657962792098201600_n.jpg?_nc_cat=110&ccb=1-7&_nc_sid=174925&_nc_ohc=jTfRAQ_PSkQAX9Ud4Ft&_nc_ht=scontent.fuln6-2.fna&oh=00_AT9sk0OI5TXeT3NoS2ulpCPqrmoEWl4IyOmugV_v74xAwA&oe=63652A63"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Тунгалаггэгээ
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >

          <v-card class="overflow-y-auto" height="150">
            <v-btn color="green" class="font-weight-bold" rounded text
              >хуур грүпп</v-btn
            >
            <v-card-text>
              UI/UX figma дээр жоохоон л Веб - C, C++ - html, css, javascript -
              react - nodejs - express - mongo/mysql - typing - бие дааж сурах
              зөвлөгөө өгөх (source-ууд) - мотивацжуулах - англи хэл - чадвар
              дээрээ суурилан хичээл заах
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >

      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t1.15752-9/310651589_508066374112800_2998084115278521601_n.jpg?_nc_cat=106&ccb=1-7&_nc_sid=ae9488&_nc_ohc=BI0FN16xvfIAX8Kai4K&_nc_ht=scontent.fuln1-2.fna&oh=03_AVKvdhfXv0GsXuSnt84xtZMvRG-kjIPyvk-r5dA2Y2eBAQ&oe=6366487B"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Зуунбилэг
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-actions class="d-flex justify-center">
              <v-btn color="green" class="font-weight-bold" rounded text
                >Golomt bank</v-btn
              >
              <v-btn color="green" class="font-weight-bold" rounded text
                >Shoppy.mn</v-btn
              >
            </v-card-actions>
            <v-card-actions class="d-flex justify-center">
              <v-btn color="green" class="font-weight-bold" rounded text
                >Smartstore.mn</v-btn
              >
              <v-btn color="green" class="font-weight-bold" rounded text
                >Xiaomi.mn</v-btn
              >
            </v-card-actions>

            <v-card-text class="text-center">
              Frontend (Vuejs, Nuxtjs, Vuetify, Tailwind) <br />
              + <br />
              Backend (Google firebase, MongoDB, ExpressJS, Django, AWS) <br />
              = <br />
              Fullstack <br />
              <div class="font-weight-bold white--text d-flex justify-center">
                Асуугаад үзвэл мэдэж л байна...
              </div>
            </v-card-text>
            <div class="d-flex justify-center">
              <v-btn color="success" text @click="bobo = !bobo">...</v-btn>
            </div>
            <v-snackbar v-model="bobo">
              Заа уучлаарай жаахан залхуурсан болно.

              <template v-slot:action="{ attrs }">
                <v-btn color="pink" text v-bind="attrs" @click="bobo = !bobo">
                  Аан за
                </v-btn>
              </template>
            </v-snackbar>
          </v-card>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >

      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t39.30808-6/283154137_1896921630505727_13492333463629676_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=Ry6zMvw67DsAX9HdjTt&_nc_ht=scontent.fuln1-2.fna&oh=00_AT_vWSTAQg30IN7Y7WAiwan0zKOUNXikRndYx-J9YtXZoQ&oe=6343A831"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Цэнгүүн
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              Веб <br />
              - C, C++ <br />
              - html, css, javascript <br />
              - react <br />
              - nodejs <br />
              - express <br />
              - mongo/mysql<br />
              - typing <br />
              - бие дааж сурах зөвлөгөө өгөх (source-ууд) <br />
              - мотивацжуулах <br />
              - англи хэл <br />
              - чадвар дээрээ суурилан хичээл заах <br />
            </v-card-text>
          </v-card>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
    </v-row>
    <v-row>
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://mir-s3-cdn-cf.behance.net/project_modules/1400/843e46150950877.631de683c2507.png"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Даваажаргал
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              Web app хөгжүүлэх сонирхолтой. Ерөнхийдөө Frontend хөгжүүлдэг.
              React, javascript анхан шатны зөвлөгөө өгөөд туслаад явна.
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      ><v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t39.30808-1/250300155_1496527717391678_4445818962569404134_n.jpg?stp=dst-jpg_p320x320&_nc_cat=110&ccb=1-7&_nc_sid=7206a8&_nc_ohc=v0J4tnCsnQkAX9IcWI3&_nc_ht=scontent.fuln1-2.fna&oh=00_AT8UyZlesvM_L9ndZsiHSl-C_CTwO76irnL--v99wWFU2A&oe=63438C51"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Саруулмаа
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card height="150" class="overflow-y-auto">
            <v-card-text>
              Сайн байна уу? Hackum Student клубийн нарийн бичиг Саруулмаа
              байна. График дизайнд сонирхолтой тул гар утасны апп болон вэб
              дизайн Figma ашиглан хийх болон найзуудтайгаа хамт цагийг өнгөрөөх
              дуртай.
            </v-card-text>
          </v-card>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >

      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t39.30808-6/301779540_1062984291023567_205441150321481504_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=174925&_nc_ohc=SHAknRbmAM0AX8oAxPo&_nc_ht=scontent.fuln1-2.fna&oh=00_AT8OeEIIVuCEXDmy2zpqxJ_7oejZhfLDXbqFlQP3CieriA&oe=63443CFB"
          ></v-img>

          <v-card-title class="d-flex justify-center" primary-title>
            Намуунцэцэг
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              Бизнесийн сургуулийн Менежментийн 4р түвшний оюутан. <br />
              <br />
              - Бизнес модел гаргана. <br />
              - Бизнесийн шинжилгээнүүд хийнэ. <br />
              - Pitch хийнэ
            </v-card-text>
          </v-card>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn
                    color="green"
                    @click="
                      (sanal = !sanal), (helo = !helo), writeUserData('ss')
                    "
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >

      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t39.30808-1/310997444_3413478762271158_8623339590520083692_n.jpg?stp=dst-jpg_s320x320&_nc_cat=100&ccb=1-7&_nc_sid=7206a8&_nc_ohc=ae3NGgaz-dYAX8bTolo&_nc_ht=scontent.fuln1-2.fna&oh=00_AT-hVqoDRe4_Y88SBBNG6LtKYiG_32yZWf-d1La8QgVi8A&oe=63452348"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Саруул
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              КУ - 3р күрс, машин сургалт, ethical hacking, код бичих, эмзэг
              байдлын судалгаа тал дээр мэнтор хийж чадна.
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln6-2.fna.fbcdn.net/v/t39.30808-6/286930792_1402487643601003_3484123559161236477_n.jpg?_nc_cat=104&ccb=1-7&_nc_sid=174925&_nc_ohc=K5z9IeWpzPwAX91Fmx0&_nc_ht=scontent.fuln6-2.fna&oh=00_AT_3MVMbWy9bH__6NbtLHKUvvqx-g2zqf2tzvU5cPUgwHw&oe=6345356F"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Мэндсайхан
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              NextJS MySQL C# Flutter Wordpress Java
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      ><v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln6-2.fna.fbcdn.net/v/t39.30808-1/305808082_5488321707953854_3342945917239222916_n.jpg?stp=dst-jpg_p320x320&_nc_cat=103&ccb=1-7&_nc_sid=7206a8&_nc_ohc=JFsDR_V8HIQAX_sAdv2&_nc_ht=scontent.fuln6-2.fna&oh=00_AT9RdWAaDE-Qu6IA0tACTfFTf1trdVvS6BDQi0eIsc5WOQ&oe=634465A6"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Сүглэгмаа
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow" height="150">
            <v-card-text> Project manager </v-card-text>
          </v-card>

          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
    </v-row>

    <v-row>
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t39.30808-6/307505977_3040897042722709_1686564949089907199_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=TYH6h5GRddcAX_2xmHi&tn=BHYNS4BHRx08ey4S&_nc_ht=scontent.fuln1-2.fna&oh=00_AT_uQc0SiLvbzzOkdkOR1xNqGD5jN6eJpI7LIQhzvlFnrA&oe=63441A8C"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Жамба
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-hidden" height="150">
            <v-card-actions class="d-flex justify-center">
              <v-btn color="green" class="font-weight-bold" rounded text
                >Zochil technology</v-btn
              >
              <v-btn color="green" class="font-weight-bold" rounded text
                >Mobicom</v-btn
              >
            </v-card-actions>
            <v-card-text>
              AWS, Docker, Express, React, Next js, Java, Python, Flutter, React
              native, Spring
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://scontent.fuln1-2.fna.fbcdn.net/v/t1.6435-9/197923928_2984035345177259_7587586923618250759_n.jpg?_nc_cat=100&ccb=1-7&_nc_sid=09cbfe&_nc_ohc=VtnBf_mOu9EAX9sHskD&_nc_ht=scontent.fuln1-2.fna&oh=00_AT_Gk-EvmpRXjhQBrZT5unFzIEBnRAJAEJ7FVbgXaj-hIA&oe=63656839"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Есүй
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card class="overflow-y-auto" height="150">
            <v-card-text>
              ХШУИС-ийн 2-р түвшний оюутан. Мэдээллийн технологи чиглэлээр
              суралцдаг. Олон газар цагийн болон үндсэн ажил хийж үзсэн. Хэрхэн
              байгууллагуудад өөрийгөө зөвөөр таниулж ажилд орох, ажлаа хаанаас
              хайх талаар сайн мэдээлэл өгч чадна. Ер нь л юу ч байсан тусалж
              дэмжиж мэдэхгүй байгаа зүйлийг чинь өөрөө мэдэхгүй байсан ч олоод
              өгч чаднаа.
            </v-card-text></v-card
          >
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://i.natgeofe.com/k/75ac774d-e6c7-44fa-b787-d0e20742f797/giant-panda-eating_3x2.jpg"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Ба бусад...
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card-text> </v-card-text>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
    </v-row>
    <v-row> </v-row>
    <!--
    <v-row>
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://i.natgeofe.com/k/75ac774d-e6c7-44fa-b787-d0e20742f797/giant-panda-eating_3x2.jpg"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Б.Зуунбилэг
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card-text>
            UI/UX figma дээр жоохоон л Веб - C, C++ - html, css, javascript -
            react - nodejs - express - mongo/mysql - typing - бие дааж сурах
            зөвлөгөө өгөх (source-ууд) - мотивацжуулах - англи хэл - чадвар
            дээрээ суурилан хичээл заах
          </v-card-text>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://i.natgeofe.com/k/75ac774d-e6c7-44fa-b787-d0e20742f797/giant-panda-eating_3x2.jpg"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Б.Зуунбилэг
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card-text>
            UI/UX figma дээр жоохоон л Веб - C, C++ - html, css, javascript -
            react - nodejs - express - mongo/mysql - typing - бие дааж сурах
            зөвлөгөө өгөх (source-ууд) - мотивацжуулах - англи хэл - чадвар
            дээрээ суурилан хичээл заах
          </v-card-text>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn color="green" @click="(sanal = !sanal), (helo = !helo)"
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      >
      <v-col cols="12" md="4"
        ><v-card>
          <v-img
            height="200"
            src="https://i.natgeofe.com/k/75ac774d-e6c7-44fa-b787-d0e20742f797/giant-panda-eating_3x2.jpg"
          ></v-img>
          <v-card-title class="d-flex justify-center" primary-title>
            Б.Зуунбилэг
          </v-card-title>
          <v-divider class="mx-4"></v-divider>
          <v-card-subtitle class="text-center"
            >Core member
            <v-icon color="green "
              >mdi-card-account-details-outline</v-icon
            ></v-card-subtitle
          >
          <v-card-text>
            UI/UX figma дээр жоохоон л Веб - C, C++ - html, css, javascript -
            react - nodejs - express - mongo/mysql - typing - бие дааж сурах
            зөвлөгөө өгөх (source-ууд) - мотивацжуулах - англи хэл - чадвар
            дээрээ суурилан хичээл заах
          </v-card-text>
          <v-expansion-panels>
            <v-expansion-panel elevation="0">
              <v-expansion-panel-header class="green--text"
                ><div>
                  Багийн гишүүд
                  <v-icon color="green "
                    >mdi-card-account-details-outline</v-icon
                  >
                </div>
              </v-expansion-panel-header>
              <v-expansion-panel-content
                ><v-form>
                  <v-text-field
                    clearable
                    label="Таны нэр"
                    single-line
                    color="green"
                  ></v-text-field>
                  <v-text-field
                    clearable
                    label="Таны утасны дугаар"
                    single-line
                    color="green"
                  ></v-text-field>
                </v-form>
                <div v-if="!sanal" class="d-flex justify-center pa-10">
                  <v-btn
                    color="green"
                    @click="
                      (sanal = !sanal), (helo = !helo), writeUserData(Zuna)
                    "
                    >Багт нэгдэх</v-btn
                  >
                </div>
              </v-expansion-panel-content>

              <v-snackbar v-model="helo">
                {{ text }} <v-icon color="green">mdi-account-check</v-icon>

                <template v-slot:action="{ attrs }">
                  <v-btn color="pink" text v-bind="attrs" @click="helo = !helo">
                    Cool
                  </v-btn>
                </template>
              </v-snackbar>
              <div v-if="sanal" class="d-flex justify-center">
                <v-card-title primary-title color="green">
                  Та санал өгсөн байна <v-icon>mdi-check-decagram</v-icon>
                </v-card-title>
              </div>
            </v-expansion-panel>
          </v-expansion-panels>
        </v-card></v-col
      > -->
    <!-- </v-row> -->
  </v-container>
</template>

<script>
// import { getDatabase, ref, onValue } from "firebase/database";
import Membercard from "../components/membercard.vue";
export default {
  components: { Membercard },
  data() {
    return {
      sanal: false,
      helo: false,
      text: `Таны саналыг хүлээн авлаа`,
      Abe: "Abe",
      Dabuna: "Dabuna",
      Davaajargal: "Davaajargal",
      Gegee: "Gegee",
      Jamba: "Jamba",
      Mendsaikhan: "Mendsaikhan",
      Namuun: "Namuun",
      Saruul: "Saruul",
      Saruulmaa: "Saruulmaa",
      Sugleg: "Sugleg",
      Tseku: "Tseku",
      Tselmuun: "Tselmuun",
      Ulambayr: "Ulambayr",
      Zuna: "pmWcQzNHXbmvJobZshHG",
      yvuul: null,
      bobo: false,
    };
  },
  // methods: {
  //   writeUserData(core) {
  //     console.log("aaa");
  //     console.log(this.$fire.database);
  //     this.$fire.firestore.addDoc("kids/5OJnx6A1jsiMSCUTumk4/", {
  //       age: "Last",
  //     });
  //   },
  // },
};
</script>
