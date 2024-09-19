/* author: https://codepen.io/jcoulterdesign/pen/ZxXbeP
Jamie Coulter
 */

@import url("https://fonts.googleapis.com/css?family=Montserrat:300,400,700");
.solar_systm {
  transform-style: preserve-3d;
  pointer-events: none;
  height: 100%;
  position: absolute;
  left: 0;
  right: 0;
}

* {
  -webkit-user-select: none;
  /* Chrome all / Safari all */
  -moz-user-select: none;
  /* Firefox all */
  -ms-user-select: none;
  /* IE 10+ */
  user-select: none;
  /* Likely future */
}

body .solar_systm .planet, body input[type=radio][name=planet]::after, body .overlay {
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
  margin: auto;
}

body .solar_systm .planet.neptune .trajectory.ner, body .solar_systm .planet.neptune .trajectory.pro, body .solar_systm .planet.neptune .trajectory.tri, body .solar_systm .planet.uranus .trajectory.umb, body .solar_systm .planet.uranus .trajectory.ari, body .solar_systm .planet.uranus .trajectory.mir, body .solar_systm .planet.saturn .trajectory.enc, body .solar_systm .planet.saturn .trajectory.di, body .solar_systm .planet.saturn .trajectory.ti, body .solar_systm .planet.jupiter .trajectory.ga, body .solar_systm .planet.jupiter .trajectory.eu, body .solar_systm .planet.jupiter .trajectory.lop, body .solar_systm .planet.mars .trajectory.p, body .solar_systm .planet.mars .trajectory.d, body .solar_systm .planet.earth .trajectory.m {
  border: 2px dashed white;
  position: absolute;
  border-radius: 3400px;
  background: none !important;
  z-index: -2;
}

body .solar_systm .planet {
  height: 1200px;
  width: 1200px;
  border-radius: 600px;
  background: red;
  transition: transform 2.8s 0.23s cubic-bezier(0.33, 0, 0, 1), opacity 2s 0.8s, box-shadow 0s 0s;
  background-size: 1140px 910px !important;
  top: auto;
  bottom: -920px;
}
body .solar_systm .planet .moon {
  height: 200px;
  width: 200px;
  border-radius: 600px;
  background: red;
  position: absolute;
  text-align: center;
  color: white;
  text-transform: uppercase;
  opacity: 0;
  transition: all 0.6s 0.2s;
}
body .solar_systm .planet .moon h2 {
  font-weight: 100;
  font-size: 40px;
  letter-spacing: 5px;
  margin: 0;
  position: relative;
  top: -120px;
}
body .solar_systm .planet .moon h3 {
  font-weight: 100;
  font-size: 20px;
  letter-spacing: 5px;
  color: #fea082;
  margin: 0;
  position: relative;
  top: -120px;
}
@keyframes planet {
  from {
    background-position-y: 0px;
  }
  to {
    background-position-y: -1000px;
  }
}

body .solar {
  position: absolute;
  transform: rotatex(-20deg);
  perspective: 800px;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
}

body input[type=radio][name=planet]::after {
  width: 220px;
  height: 220px;
  border-radius: 550px;
  appearance: none;
  outline: none;
  cursor: pointer;
  z-index: 12;
  left: 18px;
  bottom: 282px;
}

body {
  overflow: hidden;
  background: black;
  height: 100vh;
  font-family: "Montserrat", sans-serif;
}
body .logo {
  color: white;
  position: absolute;
  top: 40px;
  left: 0;
  right: 0;
  margin: auto;
  text-align: center;
  font-size: 14px;
  text-transform: uppercase;
  font-weight: 100;
  letter-spacing: 4px;
}
body .logo span {
  font-size: 12px;
  color: #f39041;
  display: block;
}
body label {
  cursor: pointer;
}
body label.mercury > .preview {
  background: url("https://www.solarsystemscope.com/images/textures/full/2k_makemake_fictional.jpg") !important;
}
body label.venus > .preview {
  background: url("https://nasa3d.arc.nasa.gov/shared_assets/images/ven0aaa2/ven0aaa2-copy-428-321.jpg") !important;
}
body label.earth > .preview {
  background: url("https://img00.deviantart.net/04ef/i/2009/114/3/e/new_earth_texture_map_by_lightondesigns.jpg") !important;
}
body label.mars > .preview {
  background: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/217233/mars_texture.jpg") !important;
}
body label.jupiter > .preview {
  background: url("https://www.jpl.nasa.gov/spaceimages/images/largesize/PIA07782_hires.jpg") !important;
}
body label.saturn > .preview {
  background: url("https://www.solarsystemscope.com/images/textures/full/2k_saturn.jpg") !important;
}
body label.uranus > .preview {
  background: url("https://img00.deviantart.net/957c/i/2017/165/4/9/uranus_texture_map_by_jcpag2010-db7yjwb.png") !important;
}
body label.neptune > .preview {
  background: url("https://img00.deviantart.net/f068/i/2017/165/b/c/neptune_texture_map_by_jcpag2010-dbcjcv5.png") !important;
}
body label.pluto > .preview {
  background: url("https://pre00.deviantart.net/4677/th/pre/f/2015/314/4/e/pluto_map__2015_nov_10__by_snowfall_the_cat-d918tlb.png") !important;
}
body label.menu {
  color: white;
  display: block;
  position: absolute;
  cursor: pointer;
  left: 90px;
  z-index: 2;
}
body label.menu:after {
  display: block;
  width: 12px;
  height: 12px;
  border: 2px solid white;
  border-radius: 60px;
  content: "";
  z-index: 2;
  position: absolute;
  top: -4px;
  left: -4px;
}
body label.menu:hover h2, body label.menu:hover h3 {
  opacity: 1;
}
body label.menu.mercury h2 .pip {
  background: #E8927C;
}
body label.menu.venus h2 .pip {
  background: #b45d15;
}
body label.menu.earth h2 .pip {
  background: #26daaa;
}
body label.menu.mars h2 .pip {
  background: #e55f45;
}
body label.menu.jupiter h2 .pip {
  background: orange;
}
body label.menu.saturn h2 .pip {
  background: #b29d81;
}
body label.menu.uranus h2 .pip {
  background: #8dcdd8;
}
body label.menu.neptune h2 .pip {
  background: #4f83e2;
}
body label.menu.pluto h2 .pip {
  background: #FF8732;
}
body label.menu .preview {
  width: 30px;
  height: 30px;
  background: yellow;
  float: left;
  background-size: auto 100% !important;
  position: absolute;
  border-radius: 100px;
  box-shadow: 0 -13px 10px 2px black inset;
}
body label.menu .info {
  position: relative;
  left: 50px;
  top: 1px;
}
body label.menu h2,
body label.menu h3 {
  text-transform: uppercase;
  margin: 0;
  font-weight: 100;
  letter-spacing: 2px;
}
body label.menu h2 {
  font-size: 11px;
  opacity: 0.4;
  margin-bottom: 4px;
}
body label.menu h2 .pip {
  width: 0;
  height: 9px;
  background: #fea082;
  float: left;
  position: relative;
  top: 3px;
  transition: all 0.3s;
  margin-right: 0px;
}
body label.menu h3 {
  font-size: 8px;
  letter-spacing: 1px;
  transition: all 0.3s;
  opacity: 0.3;
}
body label.menu:nth-of-type(1) {
  top: calc(50vh + 100px + ((14px + 34px) * 1) + 0px - 369px);
}
body label.menu:nth-of-type(2) {
  top: calc(50vh + 100px + ((14px + 34px) * 2) + 0px - 369px);
}
body label.menu:nth-of-type(3) {
  top: calc(50vh + 100px + ((14px + 34px) * 3) + 0px - 369px);
}
body label.menu:nth-of-type(4) {
  top: calc(50vh + 100px + ((14px + 34px) * 4) + 0px - 369px);
}
body label.menu:nth-of-type(5) {
  top: calc(50vh + 100px + ((14px + 34px) * 5) + 0px - 369px);
}
body label.menu:nth-of-type(6) {
  top: calc(50vh + 100px + ((14px + 34px) * 6) + 0px - 369px);
}
body label.menu:nth-of-type(7) {
  top: calc(50vh + 100px + ((14px + 34px) * 7) + 0px - 369px);
}
body label.menu:nth-of-type(8) {
  top: calc(50vh + 100px + ((14px + 34px) * 8) + 0px - 369px);
}
body label.menu:nth-of-type(9) {
  top: calc(50vh + 100px + ((14px + 34px) * 9) + 0px - 369px);
}
body input.read {
  display: none;
}
body .read:checked + label + input + .panel {
  right: 0;
}
body .read:checked + label {
  width: calc(100% - 420px);
}
body .read:checked + label::after {
  opacity: 1;
  left: 0;
}
body .read:checked + label + label {
  transition: all 0.3s 0.6s;
  opacity: 1;
}
body .read:not(:checked) + label + label {
  transition: all 0.3s 0s;
  opacity: 0;
}
body label.close {
  position: absolute;
  right: 60px;
  opacity: 0;
  transition: all 0.3s 0.4s;
  z-index: 3;
  top: 65px;
}
body label.closeBig {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 3;
  height: 100vh;
  transition: all 0.2s;
  z-index: 10;
  width: 0;
  background: rgba(56, 37, 99, 0.38);
}
body label.closeBig::after {
  content: "Back";
  text-align: center;
  font-size: 30px;
  color: white;
  position: absolute;
  left: -140px;
  opacity: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}
body .overlay {
  border-bottom: 1020px solid black;
  width: 1800px;
  height: 620px;
  top: auto;
  -webkit-transform: none;
  transform: none;
  top: -240px;
  left: -303px;
  opacity: 1;
  border-radius: 100%;
  z-index: 0;
  box-shadow: 0px -190px 215px 110px black inset;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet1:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet1:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet_description h2,
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet_description p,
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(1) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -2;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -3;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -4;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-16100px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -5;
}
body input[type=radio][name=planet].planet1:checked + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-18400px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -6;
}
body input[type=radio][name=planet].planet1:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet1:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet1:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet1:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet1:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet1:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet1:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet1:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet1:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet1:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet1:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet1:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet1:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet1:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet2:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet2:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet_description h2,
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet_description p,
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(2) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -2;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -3;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -4;
}
body input[type=radio][name=planet].planet2:checked + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-16100px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -5;
}
body input[type=radio][name=planet].planet2:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet2:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet2:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet2:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet2:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet2:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet2:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet2:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet2:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet2:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet2:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet2:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet2:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet2:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet3:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet3:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet_description h2,
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet_description p,
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -2;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -3;
}
body input[type=radio][name=planet].planet3:checked + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -4;
}
body input[type=radio][name=planet].planet3:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet3:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet3:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet3:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet3:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet3:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet3:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet3:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet3:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet3:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet3:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet3:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet3:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet3:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet4:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet4:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet_description h2,
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet_description p,
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -2;
}
body input[type=radio][name=planet].planet4:checked + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -3;
}
body input[type=radio][name=planet].planet4:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet4:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet4:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet4:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet4:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet4:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet4:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet4:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet4:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet4:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet4:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet4:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet4:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet4:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet5:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 6;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet_description h2,
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet_description p,
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet5:checked + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -2;
}
body input[type=radio][name=planet].planet5:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet5:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet5:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet5:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet5:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet5:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet5:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet5:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet5:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet5:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet5:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet5:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet5:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet5:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet6:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 7;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 6;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet_description h2,
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet_description p,
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet6:checked + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: -1;
}
body input[type=radio][name=planet].planet6:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet6:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet6:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet6:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet6:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet6:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet6:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet6:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet6:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet6:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet6:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet6:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet6:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet6:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet7:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 8;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 7;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 6;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet_description h2,
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet_description p,
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet7:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 0;
}
body input[type=radio][name=planet].planet7:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet7:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet7:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet7:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet7:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet7:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet7:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet7:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet7:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet7:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet7:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet7:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet7:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet7:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet8:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(16100px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 9;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 8;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 7;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 6;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet_description h2,
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet_description p,
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet8:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 1;
}
body input[type=radio][name=planet].planet8:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet8:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet8:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet8:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet8:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet8:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet8:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet8:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet8:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet8:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet8:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet8:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet8:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet8:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body input[type=radio][name=planet] {
  appearance: none;
}
body input[type=radio][name=planet]::after {
  content: "";
}
body input[type=radio][name=planet].planet9:checked::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input::after {
  display: none;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) {
  pointer-events: all;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(18400px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 10;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(16100px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 9;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(13800px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 8;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(11500px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 7;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(9200px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 6;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(6900px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 5;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(4600px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 4;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(2300px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 3;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scaleX(0.89);
  opacity: 2;
  animation: planet 60s 3.9s infinite linear;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet_description {
  opacity: 1;
  transition: all 0.6s 2.6s;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet_description h2,
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet_description h1 {
  position: relative;
  top: 0px;
  transition: all 0.5s 3s;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet_description p,
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet_description a {
  transition: all 1s 3.5s, padding 0.3s 0s;
  opacity: 1;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet .moon {
  opacity: 1;
  transition: all 1s 3.2s;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet .trajectory {
  opacity: 0.2;
  transition: all 0.6s 2.9s;
}
body input[type=radio][name=planet].planet9:checked + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + input + label + div .solar_systm:nth-of-type(9) .planet .overlay {
  opacity: 1;
  top: -240px;
}
body input[type=radio][name=planet].planet9:checked + label.mercury > .info h3 {
  color: #E8927C;
}
body input[type=radio][name=planet].planet9:checked + label.venus > .info h3 {
  color: #b45d15;
}
body input[type=radio][name=planet].planet9:checked + label.earth > .info h3 {
  color: #26daaa;
}
body input[type=radio][name=planet].planet9:checked + label.mars > .info h3 {
  color: #e55f45;
}
body input[type=radio][name=planet].planet9:checked + label.jupiter > .info h3 {
  color: orange;
}
body input[type=radio][name=planet].planet9:checked + label.saturn > .info h3 {
  color: #b29d81;
}
body input[type=radio][name=planet].planet9:checked + label.uranus > .info h3 {
  color: #8dcdd8;
}
body input[type=radio][name=planet].planet9:checked + label.neptune > .info h3 {
  color: #4f83e2;
}
body input[type=radio][name=planet].planet9:checked + label.pluto > .info h3 {
  color: #FF8732;
}
body input[type=radio][name=planet].planet9:checked + label {
  opacity: 1;
}
body input[type=radio][name=planet].planet9:checked + label:before {
  display: block;
  width: 4px;
  height: 4px;
  position: absolute;
  left: 2px;
  top: 2px;
  z-index: 2;
  background: white;
  border-radius: 4px;
  content: "";
}
body input[type=radio][name=planet].planet9:checked + label > .info h2 {
  opacity: 1;
}
body input[type=radio][name=planet].planet9:checked + label > .info h2 .pip {
  width: 30px;
  margin-right: 6px;
}
body input[type=radio][name=planet].planet9:checked + label > .info h3 {
  opacity: 1;
  color: #fea082;
}
body .solar_systm:nth-of-type(1) .planet {
  transform: translateZ(0px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: 2;
}
body .solar_systm:nth-of-type(1) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(1) .planet_description p,
body .solar_systm:nth-of-type(1) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(1) .planet_description h1,
body .solar_systm:nth-of-type(1) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(2) .planet {
  transform: translateZ(-2300px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: 1;
}
body .solar_systm:nth-of-type(2) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(2) .planet_description p,
body .solar_systm:nth-of-type(2) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(2) .planet_description h1,
body .solar_systm:nth-of-type(2) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(3) .planet {
  transform: translateZ(-4600px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: 0;
}
body .solar_systm:nth-of-type(3) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(3) .planet_description p,
body .solar_systm:nth-of-type(3) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(3) .planet_description h1,
body .solar_systm:nth-of-type(3) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(4) .planet {
  transform: translateZ(-6900px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -1;
}
body .solar_systm:nth-of-type(4) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(4) .planet_description p,
body .solar_systm:nth-of-type(4) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(4) .planet_description h1,
body .solar_systm:nth-of-type(4) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(5) .planet {
  transform: translateZ(-9200px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -2;
}
body .solar_systm:nth-of-type(5) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(5) .planet_description p,
body .solar_systm:nth-of-type(5) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(5) .planet_description h1,
body .solar_systm:nth-of-type(5) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(6) .planet {
  transform: translateZ(-11500px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -3;
}
body .solar_systm:nth-of-type(6) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(6) .planet_description p,
body .solar_systm:nth-of-type(6) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(6) .planet_description h1,
body .solar_systm:nth-of-type(6) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(7) .planet {
  transform: translateZ(-13800px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -4;
}
body .solar_systm:nth-of-type(7) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(7) .planet_description p,
body .solar_systm:nth-of-type(7) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(7) .planet_description h1,
body .solar_systm:nth-of-type(7) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(8) .planet {
  transform: translateZ(-16100px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -5;
}
body .solar_systm:nth-of-type(8) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(8) .planet_description p,
body .solar_systm:nth-of-type(8) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(8) .planet_description h1,
body .solar_systm:nth-of-type(8) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(9) .planet {
  transform: translateZ(-18400px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -6;
}
body .solar_systm:nth-of-type(9) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(9) .planet_description p,
body .solar_systm:nth-of-type(9) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(9) .planet_description h1,
body .solar_systm:nth-of-type(9) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm:nth-of-type(10) .planet {
  transform: translateZ(-20700px) translateY(0) rotatex(4deg) scalex(0.89);
  opacity: -7;
}
body .solar_systm:nth-of-type(10) .planet_description {
  opacity: 1;
}
body .solar_systm:nth-of-type(10) .planet_description p,
body .solar_systm:nth-of-type(10) .planet_description a {
  opacity: 0;
}
body .solar_systm:nth-of-type(10) .planet_description h1,
body .solar_systm:nth-of-type(10) .planet_description h2 {
  position: relative;
  top: -330px;
  transition: all 0.5s 0s;
}
body .solar_systm .planet .trajectory {
  transition: all 0.6s 0s;
  opacity: 0;
}
body .solar_systm .planet.mercury {
  background: url("https://www.solarsystemscope.com/images/textures/full/2k_makemake_fictional.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px rgba(188, 143, 127, 0.6);
}
body .solar_systm .planet.venus {
  background: url("https://nasa3d.arc.nasa.gov/shared_assets/images/ven0aaa2/ven0aaa2-copy-428-321.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px #ffcb9c inset, 0 0px 23px 4px #ffcb9c inset, 0 -10px 130px #b85a07;
}
body .solar_systm .planet.earth {
  background: url("https://img00.deviantart.net/04ef/i/2009/114/3/e/new_earth_texture_map_by_lightondesigns.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px #8cbaff inset, 0 0px 23px 4px #8cbaff inset, 0 -10px 130px #7894a9;
}
body .solar_systm .planet.earth .trajectory.m {
  width: 1500px;
  height: 1500px;
  left: -150px;
  top: -110px;
}
body .solar_systm .planet.earth .moon {
  left: 800px;
  top: -160px;
  transform: scale(0.45);
  background: url("https://img2.cgtrader.com/items/702173/682fad2a11/92k-moon-color-map-3d-model.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.earth .moon h3 {
  color: #26daaa;
}
body .solar_systm .planet.mars {
  background: url("https://s3-us-west-2.amazonaws.com/s.cdpn.io/217233/mars_texture.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px #e86363 inset, 0 0px 23px 4px #e86363 inset, 0 -10px 130px #6b261a;
}
body .solar_systm .planet.mars .moon h3 {
  color: #e55f45;
}
body .solar_systm .planet.mars .deimos {
  left: 900px;
  top: -100px;
  transform: scale(0.45);
  background: url("https://www.jpl.nasa.gov/spaceimages/images/largesize/PIA07782_hires.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.mars .trajectory.d {
  width: 1770px;
  height: 1770px;
  left: -317px;
  top: -110px;
}
body .solar_systm .planet.mars .trajectory.p {
  width: 1600px;
  height: 1600px;
  left: -200px;
  top: -160px;
}
body .solar_systm .planet.mars .phoebos {
  left: 100px;
  top: -160px;
  transform: scale(0.5);
  background: url("https://www.jpl.nasa.gov/spaceimages/images/largesize/PIA07782_hires.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.jupiter {
  background: url("https://www.jpl.nasa.gov/spaceimages/images/largesize/PIA07782_hires.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px rgba(188, 143, 127, 0.6);
}
body .solar_systm .planet.jupiter .moon h3 {
  color: orange;
}
body .solar_systm .planet.jupiter .trajectory.lop {
  width: 1500px;
  height: 1500px;
  left: -210px;
  top: -189px;
}
body .solar_systm .planet.jupiter .trajectory.eu {
  width: 1530px;
  height: 1530px;
  left: -165px;
  top: -130px;
}
body .solar_systm .planet.jupiter .trajectory.ga {
  width: 1760px;
  height: 1760px;
  left: -360px;
  top: -114px;
}
body .solar_systm .planet.jupiter .lo {
  left: 100px;
  top: -100px;
  transform: scale(0.4);
  background: url("http://stevealbers.net/albers/sos/jupiter/io/io_rgb_cyl.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.jupiter .europa {
  left: 400px;
  top: -210px;
  transform: scale(0.45);
  background: url("http://i.imgur.com/ZZBiHOH.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.jupiter .ganymede {
  left: 900px;
  top: -70px;
  transform: scale(0.4);
  background: url("https://vignette.wikia.nocookie.net/planet-texture-maps/images/1/14/Ganymede.jpg/revision/latest?cb=20180104001948");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.saturn {
  background: url("https://www.solarsystemscope.com/images/textures/full/2k_saturn.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px rgba(188, 143, 127, 0.6);
}
body .solar_systm .planet.saturn .moon h3 {
  color: #b29d81;
}
body .solar_systm .planet.saturn .trajectory.ti {
  width: 1500px;
  height: 1500px;
  left: -210px;
  top: -189px;
}
body .solar_systm .planet.saturn .trajectory.di {
  width: 1530px;
  height: 1530px;
  left: -165px;
  top: -130px;
}
body .solar_systm .planet.saturn .trajectory.enc {
  width: 1760px;
  height: 1760px;
  left: -360px;
  top: -114px;
}
body .solar_systm .planet.saturn .titan {
  left: 100px;
  top: -100px;
  transform: scale(0.4);
  background: url("https://pre00.deviantart.net/bea3/th/pre/i/2017/057/7/f/titan_texture_map_8k_by_fargetanik-db0f8m0.png");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.saturn .dione {
  left: 400px;
  top: -210px;
  transform: scale(0.45);
  background: url("https://www.jpl.nasa.gov/spaceimages/images/wallpaper/PIA12577-640x350.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.saturn .enceladus {
  left: 900px;
  top: -70px;
  transform: scale(0.4);
  background: url("https://img.purch.com/w/660/aHR0cDovL3d3dy5zcGFjZS5jb20vaW1hZ2VzL2kvMDAwLzA0NC8yMzkvb3JpZ2luYWwvZW5jZWxhZHVzLW1hcC1jYXNzaW5pLmpwZw==");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.uranus {
  background: url("https://img00.deviantart.net/957c/i/2017/165/4/9/uranus_texture_map_by_jcpag2010-db7yjwb.png");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px rgba(127, 188, 171, 0.6);
}
body .solar_systm .planet.uranus .moon h3 {
  color: #8dcdd8;
}
body .solar_systm .planet.uranus .trajectory.mir {
  width: 1500px;
  height: 1500px;
  left: -210px;
  top: -189px;
}
body .solar_systm .planet.uranus .trajectory.ari {
  width: 1530px;
  height: 1530px;
  left: -165px;
  top: -130px;
}
body .solar_systm .planet.uranus .trajectory.umb {
  width: 1760px;
  height: 1760px;
  left: -360px;
  top: -114px;
}
body .solar_systm .planet.uranus .miranda {
  left: 100px;
  top: -100px;
  transform: scale(0.4);
  background: url("http://celestia.simulatorlabbs.com/CelSL/textures/medres/miranda.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.uranus .ariel {
  left: 400px;
  top: -210px;
  transform: scale(0.45);
  background: url("http://celestia.freedoors.org/Celestia-Doors/textures/medres/ariel.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.uranus .umbriel {
  left: 900px;
  top: -70px;
  transform: scale(0.4);
  background: url("http://celestia.freedoors.org/Celestia-Doors/textures/medres/titania.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.neptune {
  background: url("https://www.solarsystemscope.com/images/textures/full/2k_neptune.jpg");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px #2d4153;
}
body .solar_systm .planet.neptune .moon h3 {
  color: #4f83e2;
}
body .solar_systm .planet.neptune .trajectory.tri {
  width: 1500px;
  height: 1500px;
  left: -210px;
  top: -189px;
}
body .solar_systm .planet.neptune .trajectory.pro {
  width: 1530px;
  height: 1530px;
  left: -165px;
  top: -130px;
}
body .solar_systm .planet.neptune .trajectory.ner {
  width: 1760px;
  height: 1760px;
  left: -360px;
  top: -114px;
}
body .solar_systm .planet.neptune .triton {
  left: 100px;
  top: -100px;
  transform: scale(0.4);
  background: url("https://img00.deviantart.net/b934/i/2016/198/b/0/triton_texture_map_14k_by_fargetanik-daac9tm.png");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.neptune .proteus {
  left: 400px;
  top: -210px;
  transform: scale(0.45);
  background: url("http://2.bp.blogspot.com/-NrsDNbSk8TU/VKmLHdOgw0I/AAAAAAAAHvY/dod1Kqv2Ta8/s1600/NereidTxt2.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.neptune .nereid {
  left: 900px;
  top: -70px;
  transform: scale(0.4);
  background: url("http://4.bp.blogspot.com/-3eyaVs4az74/VKmMpLo6FYI/AAAAAAAAHvs/zK5NTllQYnk/s1600/NereidTxt.jpg");
  z-index: -1;
  box-shadow: 0px -30px 30px 10px black inset;
}
body .solar_systm .planet.pluto {
  background: url("https://pre00.deviantart.net/4677/th/pre/f/2015/314/4/e/pluto_map__2015_nov_10__by_snowfall_the_cat-d918tlb.png");
  box-shadow: 0 -590px 150px black inset, 0 0px 130px 40px rgba(234, 205, 199, 0.6) inset, 0 0px 23px 4px rgba(234, 205, 199, 0.6) inset, 0 -10px 130px #2d4153;
}
body .solar_systm .planet_description {
  width: 620px;
  text-align: center;
  position: absolute;
  margin: auto;
  left: 0;
  z-index: 2;
  right: 0;
  color: white;
  font-weight: 100;
  transition: all 0.4s 0s;
  text-transform: uppercase;
  z-index: 1;
}
body .solar_systm .planet_description.mercury a {
  color: #E8927C;
}
body .solar_systm .planet_description.mercury h2 {
  color: #f7dad3;
}
body .solar_systm .planet_description.venus a {
  color: #b45d15;
}
body .solar_systm .planet_description.venus h2 {
  color: #e99046;
}
body .solar_systm .planet_description.earth a {
  color: #26daaa;
}
body .solar_systm .planet_description.earth h2 {
  color: #7de9cc;
}
body .solar_systm .planet_description.mars a {
  color: #e55f45;
}
body .solar_systm .planet_description.mars h2 {
  color: #f2ac9e;
}
body .solar_systm .planet_description.jupiter a {
  color: orange;
}
body .solar_systm .planet_description.jupiter h2 {
  color: #ffc966;
}
body .solar_systm .planet_description.saturn a {
  color: #b29d81;
}
body .solar_systm .planet_description.saturn h2 {
  color: #d9cec0;
}
body .solar_systm .planet_description.uranus a {
  color: #8dcdd8;
}
body .solar_systm .planet_description.uranus h2 {
  color: #d9eef2;
}
body .solar_systm .planet_description.neptune a {
  color: #4f83e2;
}
body .solar_systm .planet_description.neptune h2 {
  color: #a7c1f0;
}
body .solar_systm .planet_description.pluto a {
  color: #FF8732;
}
body .solar_systm .planet_description.pluto h2 {
  color: #ffc398;
}
body .solar_systm .planet_description h1,
body .solar_systm .planet_description h2,
body .solar_systm .planet_description p,
body .solar_systm .planet_description a {
  font-weight: 100;
  font-size: 10px;
  letter-spacing: 5px;
  margin: 0;
}
body .solar_systm .planet_description h1 {
  letter-spacing: 16px;
  font-size: 34px;
}
body .solar_systm .planet_description h2,
body .solar_systm .planet_description a {
  color: #fabfad;
}
body .solar_systm .planet_description h2 {
  margin-top: 60px;
  margin-bottom: 6px;
}
body .solar_systm .planet_description p {
  line-height: 26px;
  margin-top: 14px;
  oapcity: 0.9;
  margin-bottom: 10px;
}
body .solar_systm .planet_description a {
  color: #fea082;
  font-size: 11px;
  font-weight: 500;
  padding: 0 2px 5px 0px;
  border-bottom: 2px solid;
  transition: all 0.2s;
  position: relative;
  left: 0;
}
body .solar_systm .planet_description a:hover {
  padding: 0 10px 5px 10px;
  left: -1px;
}
body .solar_systm .planet_description a span {
  letter-spacing: 0;
  margin-left: -5px;
}
body .panel {
  position: absolute;
  right: -520px;
  width: 300px;
  top: 0;
  height: 100vh;
  transition: all 0.2s;
  color: black;
  background: white;
  padding: 10px 60px 0px 60px;
  overflow: scroll;
}
body .panel body::-webkit-scrollbar {
  width: 1em;
}
body .panel body::-webkit-scrollbar-track {
  -webkit-box-shadow: inset 0 0 6px rgba(0, 0, 0, 0.3);
}
body .panel body::-webkit-scrollbar-thumb {
  background-color: darkgrey;
  outline: 1px solid slategrey;
}
body .panel .profile {
  padding-top: 4px;
}
body .panel .profile p {
  line-height: 10px;
}
body .panel .profile p span {
  font-weight: 600;
  color: black;
}
body .panel img {
  border-radius: 2px;
  width: 100%;
}
body .panel h1 {
  text-transform: uppercase;
  font-weight: 100;
  margin: 0 0 0 0;
  letter-spacing: 3px;
  top: 0;
  padding: 49px 0 0 0;
  width: 100%;
  font-size: 20px;
}
body .panel h1::after {
  width: 30px;
  height: 2px;
  background: black;
  display: block;
  content: "";
  margin-bottom: 30px;
  margin-top: 8px;
}
body .panel h2 {
  font-size: 13px;
  text-transform: uppercase;
  font-weight: 600;
  margin-top: 30px;
}
body .panel h2::after {
  width: 30px;
  height: 2px;
  background: black;
  display: block;
  content: "";
  margin-top: 8px;
}
body .panel p {
  color: #a0a0a0;
  font-size: 12px;
  line-height: 20px;
}
