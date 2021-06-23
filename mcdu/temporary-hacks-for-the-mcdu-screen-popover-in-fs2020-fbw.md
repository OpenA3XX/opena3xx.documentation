# Temporary Hacks for the MCDU Screen Popover in FS2020 FBW

```css
@import url("/CSS/A32NX_Display_Common.css");

:root {
  font-family: "HoneywellMCDU" !important;
}

@font-face {
  src: url("/Fonts/HoneywellMCDU.ttf") format("truetype");
  font-family: "HoneywellMCDU";
  font-style: normal;
  font-weight: 900;
}

@font-face {
  src: url("/Fonts/HoneywellMCDUSmall.ttf") format("truetype");
  font-family: "HoneywellMCDUSmall";
  font-style: normal;
  font-weight: 900;
}

#highlight {
  position: absolute;
  height: 100%;
  width: 100%;
  z-index: 10;
}

@keyframes TemporaryShow {
  0%,
  100% {
    visibility: visible;
  }
}

@keyframes TemporaryHide {
  0%,
  100% {
    visibility: hidden;
  }
}

#SystemTesting {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: row;
  align-items: center;
  text-align: center;
  justify-content: center;
}

#highlight {
  position: absolute;
  height: 100%;
  width: 100%;
  z-index: 10;
}

#Mainframe {
  width: 100%;
  height: 100%;
  background-color: rgb(4, 4, 5);
}

span:empty:before {
  content: " ";
}

a320-neo-cdu-main-display {
  position: absolute;
  width: 100%;
  height: 100%;
  font-family: "HoneywellMCDU" !important;
  font-size: 5.3vw !important;
  color: var(--displayWhite);
}

a320-neo-cdu-main-display div {
  font-family: "HoneywellMCDU" !important;
}

a320-neo-cdu-main-display text {
  font-family: "HoneywellMCDU" !important;
}

.white {
  color: var(--mcduWhite);
}

.inop {
  color: var(--mcduLightGrey);
}

.cyan {
  color: var(--mcduCyan);
}

.yellow {
  color: var(--mcduYellow);
}

.green {
  color: var(--mcduGreen);
}

.amber {
  color: var(--mcduAmber);
}

.red {
  color: var(--mcduRed);
}

.magenta {
  color: var(--mcduMagenta);
}

fmc-main-display::before {
  content: " ";
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background: linear-gradient(rgba(9, 13, 20, 1) 50%, rgba(9, 13, 20, 1) 50%),
    linear-gradient(
      90deg,
      rgba(9, 13, 20, 1),
      rgba(9, 13, 20, 1),
      rgba(9, 13, 20, 1)
    );
  z-index: 2;
  background-size: 100% 2px, 3px 100%;
  pointer-events: none;
}

#header {
  height: 8.1%;
  margin-top: 2.2%;
  margin-bottom: -0.3%;
  display: block;
  text-align: center;
}

#page-info {
  display: block;
  text-align: right;
  position: absolute;
  top: 7.5%;
  right: 5%;
}

#title-left {
  display: block;
  text-align: right;
  position: absolute;
  top: 7.5%;
  left: 5%;
}

.b-text {
  letter-spacing: normal;
}

.s-text,
text .s-text,
div .s-text,
span .s-text {
  font-family: HoneywellMCDUSmall, HoneywellMCDU !important;
  line-height: 1.25;
}

.b-text {
  letter-spacing: normal;
}

.msg-text {
  margin-top: 1.5% !important;
  height: 8.1% !important;
}

.msg-text.label-left {
  left: 4% !important;
}

.msg-text.label-right {
  right: 6% !important;
}

.label {
  height: 6.55%;
  margin: 0;
  white-space: pre;
}

.label-left {
  position: absolute;
  left: 4.5%;
  width: 100%;
  text-align: left;
}

.label-right {
  position: absolute;
  right: 5%;
  width: 100%;
  text-align: right;
}

.label-center {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}

.line {
  height: 6.55%;
  margin: 0;
  white-space: pre;
}

.line-left {
  position: absolute;
  left: 4%;
  width: 100%;
  text-align: left;
}

.line-right {
  position: absolute;
  right: 4%;
  width: 100%;
  text-align: right;
}

.line-center {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}

#in-out {
  padding-left: 4%;
}

#arrow-vertical {
  float: right;
}

#arrow-horizontal {
  position: absolute;
  right: 1%;
  width: 100%;
  text-align: right;
}

.left {
  margin-left: 4%;
  float: left;
}

.right {
  margin-right: 6%;
  float: right;
}

```

C:\FS2020\Community\flybywire-aircraft-a320-neo\html\_ui\Pages\VCockpit\Instruments\Airliners\FlyByWire\_A320\_Neo\CDU\A320\_Neo\_CDU.css

```text
// Panel Configuration File
// Boeing 747-400
// Copyright (c) 1999-2003 Microsoft Corporation.  All rights reserved.

[Default View]
X=0
Y=0
SIZE_X=8192
SIZE_Y=2800

[Color]
Day=255,255,255
Night=233,166,134
Luminous=201,64,64

[VCockpit01]
size_mm=1280,1280
pixel_size=1280,1280
texture=$PFD

htmlgauge00=A32NX/PFD/template.html?Index=1, 0,0,1280,1280

[VCockpit02]
size_mm=1280,1280
pixel_size=1280,1280
texture=$MFD

htmlgauge00=Airliners/FlyByWire_A320_Neo/MFD/A320_Neo_MFD.html?Index=1, 0,0,1280,1280

[VCockpit03]
size_mm=1280,1280
pixel_size=1280,1280
texture=$EICAS1

htmlgauge00=Airliners/FlyByWire_A320_Neo/EICAS/A320_Neo_EICAS.html?Index=1, 0,0,1280,1280

[VCockpit04]
size_mm=1280,1280
pixel_size=1280,1280
texture=$EICAS2

htmlgauge00=Airliners/FlyByWire_A320_Neo/EICAS/A320_Neo_EICAS.html?Index=2, 0,0,1280,1280

[VCockpit05]
size_mm=512,512
pixel_size=512,512
texture=$AttitudeDisplay

htmlgauge00=Airliners/FlyByWire_A320_Neo/SAI/A320_Neo_SAI.html, 0,0,512,512

[VCockpit06]
size_mm=256,256
pixel_size=256,256
texture=$Clock

htmlgauge00=A32NX/Clock/template.html,	0,0, 256, 256

[VCockpit07]
size_mm=512,384
pixel_size=512,384
texture=$Com
htmlgauge00=A32NX/DCDU/template.html, 0,0,512,384

[VCockpit08]
size_mm=1024,768
pixel_size=1024,768
texture=$FMC

htmlgauge00=Airliners/FlyByWire_A320_Neo/CDU/A320_Neo_CDU.html, 0,0,1024,768

[VCockpit09]
size_mm=1280,1280
pixel_size=1280,1280
texture=$FCU

htmlgauge00=Airliners/FlyByWire_A320_Neo/FCU/A320_Neo_FCU.html, 0,0,1280,1280

[VCockpit10]
size_mm=432,512
pixel_size=432,512
texture=$FDW

htmlgauge00=A32NX/RMP/template.html, 0,0,432,512

[VCockpit11]
size_mm=316,128
pixel_size=316,128
texture=$TCI

htmlgauge00=A32NX/ATC/template.html, 0,0,316,128

[VCockpit12]
size_mm=338,128
pixel_size=338,128
texture=$RTPI

htmlgauge00=A32NX/RTPI/template.html, 0,0,338,128

[VCockpit13]
size_mm=256,128
pixel_size=256,128
texture=$BAT

htmlgauge00=A32NX/BAT/template.html, 0,0,256,128

[VCockpit14]
size_mm=1280,1280
pixel_size=1280,1280
texture=$PFD2

htmlgauge00=A32NX/PFD/template.html?Index=2, 0,0,1280,1280

[VCockpit15]
size_mm=1280,1280
pixel_size=1280,1280
texture=$MFD2

htmlgauge00=Airliners/FlyByWire_A320_Neo/MFD/A320_Neo_MFD.html?Index=2, 0,0,1280,1280

[VCockpit16]
size_mm=1430,1000
pixel_size=1430,1000
texture=$EFB

htmlgauge00=A32NX/EFB/template.html, 0,0,1430,1000

[VCockpit17]
size_mm=0,0
pixel_size=0,0
texture=$PFD
background_color=0,0,0

htmlgauge00=WasmInstrument/WasmInstrument.html?wasm_module=systems.wasm&wasm_gauge=systems, 0,0,0,0
htmlgauge01=WasmInstrument/WasmInstrument.html?wasm_module=fbw.wasm&wasm_gauge=fbw, 0,0,0,0
htmlgauge02=WasmInstrument/WasmInstrument.html?wasm_module=fadec.wasm&wasm_gauge=FadecGauge, 0,0,0,0

[VPainting01]
size_mm				= 2048,512
texture				= $RegistrationNumber
location 			= exterior

painting00=Registration/Registration.html?font_color=black,	0, 0, 2048, 512

[VPainting02]
size_mm=1024,1024
pixel_size=1024,1024
texture=$PRINT
painting00=Printer/Printer.html?Index=0,	0, 0, 1024, 1024

[VPainting03]
size_mm=1024,1024
pixel_size=1024,1024
texture=$PRINT_STATIC
painting00=Printer/Printer.html?Index=1,	0, 0, 1024, 1024

```

C:\FS2020\Community\flybywire-aircraft-a320-neo\SimObjects\AirPlanes\FlyByWire\_A320\_NEO\panel\panel.cfg

