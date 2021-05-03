<template>
  <div>
    <v-container>
      <v-row>
        <v-col cols="12" sm="6" md="8">
          <div class="title">
            <v-icon size="40" @click="$router.push('/man-tshirt')">mdi-arrow-left-thick</v-icon>
            <p class="mr-2 mt-4">Unisex Jersey Short Sleeve V-Neck Tee</p>
            <v-dialog
                v-model="dialog"
                persisten      
                max-width="600px"
              >
                <template v-slot:activator="{ on, attrs }">
                  <v-btn
                    color="black"
                    outlined
                    v-bind="attrs"
                    v-on="on"
                  >
                    Preview
                  </v-btn>
                </template>
                <v-card>
                  <v-card-title>
                    <span class="headline">Preview</span>
                  </v-card-title>
                  <v-card-text>
                    <v-container>
                      <v-row justify="center">
                        <img src="~/assets/print/front-tshirt.png" style="width: 400px; height: 400px;">
                      </v-row>
                    </v-container>
                    <small>*indicates required field</small>
                  </v-card-text>
                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn
                      color="blue darken-1"
                      text
                      @click="dialog = false"
                    >
                      Close
                    </v-btn>
                  </v-card-actions>
                </v-card>
              </v-dialog>
          </div>
          <div class="print-area">

            <v-btn outlined rounded class="mr-2 mt-5" @click="preview = image1">Урд хэсэг</v-btn>
            <v-btn outlined rounded class="ml-2 mt-5" @click="preview = image2">Ард хэсэг</v-btn>
          </div>
          <div  class="print-area mt-5">
            
            <!-- nemsem -->

            <div class="area">
              <vue-resizable class="resizable" ref="resizableComponent"
                            :dragSelector="dragSelector"
                            :active="handlers" :fit-parent="fit" :maximize="maximize"
                            :max-width="checkEmpty(maxW)" :max-height="checkEmpty(maxH)"
                            :min-width="checkEmpty(minW)" :min-height="checkEmpty(minH)"
                            :width="width" :height="height"
                            :left="0" :top="0"
                            @mount="eHandler"
                            @resize:move="eHandler" @resize:start="eHandler" @resize:end="eHandler"
                            @drag:move="eHandler" @drag:start="eHandler" @drag:end="eHandler" @maximize="eHandler"
            >
                <div class="block">
                  <div class="drag-area-1" >
                      <!-- <img v-if="preview == image1 && selectedFile" :src="selectedFile" 
                      :aspect-ratio="16/9"
                      :Width="Width"/> -->
                      <v-img
                        :aspect-ratio="16/9"
                        :Width="Width"
                        v-if="preview == image1 && selectedFile" :src="selectedFile" 
                      ></v-img>
                  </div>
                        <div class="table-area">
            <table>
              <tr>
                <td>w:{{ width }}</td>
                <td>h:{{ height }}</td>
              </tr>
              <tr>
                <td>l:{{ left }}</td>
                <td>t:{{ top }}</td>
              </tr>
            </table>
          </div>
          <div class="drag-area-2">drag_2</div>
                </div>
      
              </vue-resizable>
               
            </div>
            
            <img class="image1" :src="preview" />
            <br />
            
          </div>
            <v-slider
                        v-model="width"
                        class="align-self-stretch"
                        min="200"
                        max="500"
                        step="1"
                      ></v-slider>
        </v-col>
        <v-divider vertical></v-divider>
        <v-col cols="6" md="4">
          <div class="right mt-10 ml-5">
            <img class="image" src="~/assets/print/image.png" />
            <div>
              <v-btn
                color="#25BC3D"
                class="text-none"
                round
                depressed
                :loading="isSelecting"
                @click="onButtonClick"
              >
                <v-icon left>mdi-cloud-upload-outline</v-icon>
                {{ buttonText }}
              </v-btn>
              <input
                ref="uploader"
                class="d-none"
                type="file"
                accept="image/png, image/jpeg"
                @change="onFileChanged"
              />
            </div>
            <h4>Only JPG / PNG files supported</h4>
            <p>
              Print file requirements
              <br />JPG and PNG file types supported
              <br />Maximum file size 50MB
              <br />Recommended size 3600 × 4200 px
            </p>
            <v-btn color="#25BC3D" @click="$router.push('/mystore')">Add Brand</v-btn>

            <!-- nemsen -->
            <div class="area1 table-block">
      <div class="table-row">
        <div><h4>handlers:</h4></div>
        <span v-for="handler in ['r', 'rb', 'b', 'lb', 'l', 'lt', 't', 'rt']" :key="handler">
                    {{ handler }}:<input type="checkbox" v-model="handlers" :value="handler"/>
               </span>
      </div>
      <div class="table-row">
        <div class="table-cell">
          minWidth:<input class="table-input" type="number" v-model.number="minW"/>
        </div>
        <div class="table-cell">
          maxWidth:<input class="table-input" type="number" v-model.number="maxW"/>
        </div>
      </div>
      <div class="table-row">
        <div class="table-cell">
          minHeight:<input class="table-input" type="number" v-model.number="minH"/>
        </div>
        <div class="table-cell">
          maxHeight:<input class="table-input" type="number" v-model.number="maxH"/>
        </div>
      </div>
      <div class="table-row">
        <div class="table-cell">
          width:<input class="table-input" type="number" v-model.number="width"/>
        </div>
        <div class="table-cell">
          height:<input class="table-input" type="number" v-model.number="height"/>
        </div>
      </div>
      <div class="table-row">
        <div class="table-cell">
          left:<input class="table-input" type="number" v-model.number="left"/>
        </div>
        <div class="table-cell">
          top:<input class="table-input" type="number" v-model.number="top"/>
        </div>
      </div>
      <div class="table-row">
        <div class="table-cell">
          fitParent:<input type="checkbox" v-model.number="fit"/>
        </div>
        <div class="table-cell">
          maximize:<input type="checkbox" v-model.number="maximize"/>
        </div>
      </div>
      <div class="table-row" style="text-align: left;">
        <div class="table-cell" style="padding: 0 20px;width: 100%">
          lastEvent: {{ event }}
        </div>
      </div>
    </div>

          </div>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
import Front from "../assets/print/upload-tshirt.png";
import Back from "../assets/print/upload-tshirt-back.png";
import VueResizable from "~/components/position.vue"

export default {
  name: "App",
  components: { VueResizable },
  data() {
    const tW = 150;
    const tH = 150;
    return ({
    defaultButtonText: "Create Brand",
    selectedFile: null,
    isSelecting: false,
    preview: null,
    image1: Front,
    image2: Back,
    Width: 150,
    Height:150,
    dialog: false,

    handlers: ['r', 'rb', 'b', 'lb', 'l', 'lt', 't', 'rt'],
    left: `0px`, top: `0px`,
    height: tH, width: tW,
    maxW: 250, maxH: 250,
    minW: 100, minH: 100,
    fit: true, maximize: false, event: '',
    dragSelector: ".drag-area-1, .drag-area-2"
  })
  },
  computed: {
    buttonText() {
      return this.selectedFile
        ? this.selectedFile.name
        : this.defaultButtonText;
    },
  },

  mounted() {
    this.preview = this.image1;
  },
  methods: {
    onButtonClick() {
      this.isSelecting = true;
      window.addEventListener(
        "focus",
        () => {
          this.isSelecting = false;
        },
        { once: true }
      );

      this.$refs.uploader.click();
    },
    onFileChanged(e) {
      const file = e.target.files[0];
      this.selectedFile = URL.createObjectURL(file);
      console.log(this.selectedFile);
      // do something
    },
    frontside: function () {
      this.image2 = this.image1;
    },
    backside: function () {
      this.image1 = this.image2;
    },

    eHandler(data) {
      this.width = data.width;
      this.height = data.height;
      this.left = data.left;
      this.top = data.top;
      this.event = data.eventName;
      if (data.eventName === 'maximize') {
        this.maximize = data.state;
      }
    },
    checkEmpty(value) {
      return typeof value !== "number" ? 0 : value;
    }
  },

  filters: {
    checkEmpty(value) {
      return typeof value !== "number" ? 0 : value;
    }
  }
};
</script>

<style scoped>
.block {
  height: 100%;
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
</style>
<style>
.v-image__image--cover {
  background-size: contain;
}
.title {
  width: auto;
  height: 50px;
  background-color: #c4c4c4;
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.right {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.image1 {
  width: 404px;
  height: 384px;
  z-index: 0;
}
.print-area {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  position: relative;
}
.absolute-img {
  width: 150px;
  height: 150px;
}
.image {
  width: 241px;
  height: 150px;
}


.area1 {
  width: 250px;
  height: 250px;
  display: inline-block;
  border: 1px solid #dddddd;
  background: #ffffff;
  color: #333333;;
  float: left;
  margin: 10px;
}

.area {
  position: absolute;
    z-index: 10;
    width: 100%;
    height: 100%;
    display: inline-block;
    color: #333333;
    float: left;
    margin: 10px;

}
/* 
#block1 {
  border: solid black 1px;
  height: 300px;
  width: 300px;
  display: inline-block;
  float: left;
} */

.resizable {
  width: 150px;
  height: 150px;
  padding: 0;
  font-weight: normal;
  color: #ffffff;
  position: relative;
}

.table-block {
  display: table;
}

.table-row {
  display: table-row;
  text-align: center;
}

.table-cell {
  width: 50%;
  display: inline-block
}

.table-input {
  width: 50px
}

.drag-area-1, .drag-area-2 {
  width: 100%;
  height: 100%;
  color: white;
  text-align: center;
  cursor: pointer;
}

.table-area {
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

</style>