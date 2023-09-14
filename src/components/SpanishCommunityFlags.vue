<template>
  <div v-if="comunidadData" :alt="`Bandera ${comunidadData.name} `">
    <img
      class="cover w-full h-full"
      :src="comunidadData.flag"
      :alt="`Bandera ${comunidadData.name} `"
    />
    <span v-if="showName">{{ comunidadData.name }}</span>
  </div>
</template>

<script>
import Andalucia from "../assets/Andalucía.png";
import Aragon from "../assets/Aragón.png";
import Asturias from "../assets/Asturias.png";
import Baleares from "../assets/Baleares.png";
import Canarias from "../assets/Canarias.png";
import Cantabria from "../assets/Cantabria.png";
import CastillaLaMancha from "../assets/Castilla-La-Mancha.png";
import CastillaYLeon from "../assets/Castilla-Y-Leon.png";
import Cataluna from "../assets/Cataluna.png";
import Extremadura from "../assets/Extremadura.png";
import Galicia from "../assets/Galicia.png";
import Madrid from "../assets/Madrid.png";
import Murcia from "../assets/Murcia.png";
import Navarra from "../assets/Navarra.png";
import PaisVasco from "../assets/Pais-Vasco.png";
import LaRioja from "../assets/La-Rioja.png";
import ComunidadValenciana from "../assets/Comunidad-Valenciana.png";
import Ceuta from "../assets/Ceuta.svg";
import Melilla from "../assets/Melilla.svg";
import NotDefined from "../assets/Not-Defined.png";

export default {
  props: {
    isoCode: {
      type: String,
      required: true,
    },
    showName: {
      type: Boolean,
      default: false,
    },
  },
  data() {
    return {
      comunidades: {
        AN: { name: "Andalucía", flag: Andalucia },
        AR: { name: "Aragón", flag: Aragon },
        AS: { name: "Asturias", flag: Asturias },
        IB: { name: "Baleares", flag: Baleares },
        CN: { name: "Canarias", flag: Canarias },
        CB: { name: "Cantabria", flag: Cantabria },
        CM: { name: "Castilla-La Mancha", flag: CastillaLaMancha },
        CL: { name: "Castilla y León", flag: CastillaYLeon },
        CT: { name: "Cataluña", flag: Cataluna },
        EX: { name: "Extremadura", flag: Extremadura },
        GA: { name: "Galicia", flag: Galicia },
        MD: { name: "Madrid", flag: Madrid },
        MC: { name: "Murcia", flag: Murcia },
        NC: { name: "Navarra", flag: Navarra },
        PV: { name: "País Vasco", flag: PaisVasco },
        RI: { name: "La Rioja", flag: LaRioja },
        VC: { name: "Comunidad Valenciana", flag: ComunidadValenciana },
        CE: { name: "Ceuta", flag: Ceuta },
        ML: { name: "Melilla", flag: Melilla },
        NT: { name: "No Definido", flag: NotDefined },
      },
    };
  },
  computed: {
    comunidadData() {
      return this.comunidades[this.isoCode];
    },
  },
};
</script>
