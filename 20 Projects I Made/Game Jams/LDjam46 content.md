---
title: "LDjam46 content"
source: "Game Stuff/LDjam46 content"
modified: 2020-04-19
type: reference-data
area: jam
status: "prototyped"
projects: ["[[Game Jams]]"]
concepts: ["Ludum Dare", "Tool Item Matching Game"]
words: 2584
summary: "Spreadsheet of generated Lua import_item(...) code lines for item definitions (tools like power drill, hammer) with related items and names for an LD46 game."
tags: ["area/jam", "project/game-jams", "type/reference-data"]
---

## Sheet: Sheet1

| import_item(" | power-drill | ", | 1.0 | ,{" | power-sander | "," | screwdriver | "}," | Donk Driller 9000 - Power drill | "), | import_item("power-drill",1,{"power-sander","screwdriver"},"Donk Driller 9000 - Power drill"), |
|---|---|---|---|---|---|---|---|---|---|---|---|
| import_item(" | power-sander | ", | 2.0 | ,{" | power-drill | "," | screwdriver | "}," | Super Sander 9000 - Power sander | "), | import_item("power-sander",2,{"power-drill","screwdriver"},"Super Sander 9000 - Power sander"), |
| import_item(" | tea-cup | ", | 3.0 | ,{" | screw | "," | nail | "}," | Bone china tea cup - single unit | "), | import_item("tea-cup",3,{"screw","nail"},"Bone china tea cup - single unit"), |
| import_item(" | spanner-one-sided | ", | 4.0 | ,{" | spanner-two-sided | "," | screwdriver | "}," | Singleboy - spanner | "), | import_item("spanner-one-sided",4,{"spanner-two-sided","screwdriver"},"Singleboy - spanner"), |
| import_item(" | screwdriver | ", | 5.0 | ,{" | screw | "," | nail | "}," | Screwmaster 9000 - manual screwdriver | "), | import_item("screwdriver",5,{"screw","nail"},"Screwmaster 9000 - manual screwdriver"), |
| import_item(" | trowel | ", | 6.0 | ,{" | chisel | "," | tea-cup | "}," | Brickies trowel (Anti-RSI edition) | "), | import_item("trowel",6,{"chisel","tea-cup"},"Brickies trowel (Anti-RSI edition)"), |
| import_item(" | spanner-two-sided | ", | 7.0 | ,{" | spanner-one-sided | "," | screwdriver | "}," | Doubleboy - spanner | "), | import_item("spanner-two-sided",7,{"spanner-one-sided","screwdriver"},"Doubleboy - spanner"), |
| import_item(" | wrench | ", | 8.0 | ,{" | pliers | "," | spanner-two-sided | "}," | Monkey puzzle wrench | "), | import_item("wrench",8,{"pliers","spanner-two-sided"},"Monkey puzzle wrench"), |
| import_item(" | pliers | ", | 9.0 | ,{" | wrench | "," | spanner-one-sided | "}," | Monkey grip pliers | "), | import_item("pliers",9,{"wrench","spanner-one-sided"},"Monkey grip pliers"), |
| import_item(" | hammer | ", | 10.0 | ,{" | sledge-hammer | "," | tea-cup | "}," | E-Mojolnir - Cordless hammer | "), | import_item("hammer",10,{"sledge-hammer","tea-cup"},"E-Mojolnir - Cordless hammer"), |
| import_item(" | paintbrush | ", | 11.0 | ,{" | art-brush | "," | tea-cup | "}," | Strokemaster - paintbrush | "), | import_item("paintbrush",11,{"art-brush","tea-cup"},"Strokemaster - paintbrush"), |
| import_item(" | tape-measure | ", | 12.0 | ,{" | box-cutter | "," | tea-cup | "}," | Straightedge - tape measure | "), | import_item("tape-measure",12,{"box-cutter","tea-cup"},"Straightedge - tape measure"), |
| import_item(" | box-cutter | ", | 13.0 | ,{" | hacksaw | "," | hand-saw | "}," | CuttyCutty - Box cutter | "), | import_item("box-cutter",13,{"hacksaw","hand-saw"},"CuttyCutty - Box cutter"), |
| import_item(" | paint-roller | ", | 14.0 | ,{" | trowel | "," | paintbrush | "}," | Wallpaver - Paint roller | "), | import_item("paint-roller",14,{"trowel","paintbrush"},"Wallpaver - Paint roller"), |
| import_item(" | chisel | ", | 15.0 | ,{" | trowel | "," | pick | "}," | ChippyChippy - Woodworking chisel | "), | import_item("chisel",15,{"trowel","pick"},"ChippyChippy - Woodworking chisel"), |
| import_item(" | hand-saw | ", | 16.0 | ,{" | hacksaw | "," | box-cutter | "}," | HackNoMore - Hand saw | "), | import_item("hand-saw",16,{"hacksaw","box-cutter"},"HackNoMore - Hand saw"), |
| import_item(" | hacksaw | ", | 17.0 | ,{" | hand-saw | "," | box-cutter | "}," | Smoothcut - Hacksaw | "), | import_item("hacksaw",17,{"hand-saw","box-cutter"},"Smoothcut - Hacksaw"), |
| import_item(" | screw | ", | 18.0 | ,{" | nail | "," | screwdriver | "}," | Wood screw - single unit | "), | import_item("screw",18,{"nail","screwdriver"},"Wood screw - single unit"), |
| import_item(" | nail | ", | 19.0 | ,{" | screw | "," | tea-cup | "}," | Nail (1pcs) | "), | import_item("nail",19,{"screw","tea-cup"},"Nail (1pcs)"), |
| import_item(" | axe | ", | 20.0 | ,{" | hammer | "," | pick | "}," | Lumbar Support - Wood Axe | "), | import_item("axe",20,{"hammer","pick"},"Lumbar Support - Wood Axe"), |
| import_item(" | pick | ", | 21.0 | ,{" | axe | "," | shovel | "}," | UmberPro - Pickaxe | "), | import_item("pick",21,{"axe","shovel"},"UmberPro - Pickaxe"), |
| import_item(" | shovel | ", | 22.0 | ,{" | axe | "," | pick | "}," | Diamondstar - Shovel | "), | import_item("shovel",22,{"axe","pick"},"Diamondstar - Shovel"), |
| import_item(" | sledge-hammer | ", | 23.0 | ,{" | hammer | "," | tea-cup | "}," | SimonCo Number 4 Sledgehammer | "), | import_item("sledge-hammer",23,{"hammer","tea-cup"},"SimonCo Number 4 Sledgehammer"), |
| import_item(" | pencil | ", | 24.0 | ,{" | pen | "," | marker | "}," | GeneriCo HB pencil | "), | import_item("pencil",24,{"pen","marker"},"GeneriCo HB pencil"), |
| import_item(" | pen | ", | 25.0 | ,{" | pencil | "," | marker | "}," | GeneriCo ball point pen | "), | import_item("pen",25,{"pencil","marker"},"GeneriCo ball point pen"), |
| import_item(" | marker | ", | 26.0 | ,{" | pen | "," | pencil | "}," | GeneriCo Dry erase marker | "), | import_item("marker",26,{"pen","pencil"},"GeneriCo Dry erase marker"), |
| import_item(" | art-brush | ", | 27.0 | ,{" | paintbrush | "," | quill | "}," | PinselFairy - artists paintbrush | "), | import_item("art-brush",27,{"paintbrush","quill"},"PinselFairy - artists paintbrush"), |
| import_item(" | quill | ", | 29.0 | ,{" | art-brush | "," | paintbrush | "}," | Countess quill pen | "), | import_item("quill",29,{"art-brush","paintbrush"},"Countess quill pen"), |
| import_item(" | ink-pot | ", | 30.0 | ,{" | iodine | "," | nail-polish | "}," | Black ink, pot, 115ml | "), | import_item("ink-pot",30,{"iodine","nail-polish"},"Black ink, pot, 115ml"), |
| import_item(" | palette-board | ", | 31.0 | ,{" | book-yellow | "," | book-red | "}," | Painters pinsel house brand (used) | "), | import_item("palette-board",31,{"book-yellow","book-red"},"Painters pinsel house brand (used)"), |
| import_item(" | book-yellow | ", | 34.0 | ,{" | book-red | "," | palette-board | "}," | How to label products - Yellow edition | "), | import_item("book-yellow",34,{"book-red","palette-board"},"How to label products - Yellow edition"), |
| import_item(" | book-red | ", | 35.0 | ,{" | book-yellow | "," | palette-board | "}," | 101 book titles - Red edition | "), | import_item("book-red",35,{"book-yellow","palette-board"},"101 book titles - Red edition"), |
| import_item(" | folder | ", | 36.0 | ,{" | book-red | "," | book-yellow | "}," | High tech paper storage solution - 1pcs | "), | import_item("folder",36,{"book-red","book-yellow"},"High tech paper storage solution - 1pcs"), |
| import_item(" | camera-1 | ", | 39.0 | ,{" | camera-stand | "," | maxi-lens | "}," | AlmostPro Camera | "), | import_item("camera-1",39,{"camera-stand","maxi-lens"},"AlmostPro Camera"), |
| import_item(" | mini-camera-1 | ", | 41.0 | ,{" | television-cam | "," | camera-cover | "}," | WentPro Sports camera | "), | import_item("mini-camera-1",41,{"television-cam","camera-cover"},"WentPro Sports camera"), |
| import_item(" | mini-camera-2 | ", | 42.0 | ,{" | television-cam | "," | camera-cover | "}," | WentPro Sports camera (Hero edition) | "), | import_item("mini-camera-2",42,{"television-cam","camera-cover"},"WentPro Sports camera (Hero edition)"), |
| import_item(" | camera-stand | ", | 43.0 | ,{" | camera-cover | "," | camera-1 | "}," | ProFoot camera stand | "), | import_item("camera-stand",43,{"camera-cover","camera-1"},"ProFoot camera stand"), |
| import_item(" | camera-cover | ", | 44.0 | ,{" | camera-stand | "," | camera-1 | "}," | Splash proof WentPro guard | "), | import_item("camera-cover",44,{"camera-stand","camera-1"},"Splash proof WentPro guard"), |
| import_item(" | handy-cam | ", | 45.0 | ,{" | maxi-lens | "," | tea-cup | "}," | Handycam (with foot attachment) | "), | import_item("handy-cam",45,{"maxi-lens","tea-cup"},"Handycam (with foot attachment)"), |
| import_item(" | television-cam | ", | 46.0 | ,{" | maxi-lens | "," | tea-cup | "}," | Studio Camera | "), | import_item("television-cam",46,{"maxi-lens","tea-cup"},"Studio Camera"), |
| import_item(" | profi-cam | ", | 47.0 | ,{" | maxi-lens | "," | tea-cup | "}," | ActualPro Photography device | "), | import_item("profi-cam",47,{"maxi-lens","tea-cup"},"ActualPro Photography device"), |
| import_item(" | maxi-lens | ", | 48.0 | ,{" | camera-stand | "," | camera-cover | "}," | Camera zoom lens | "), | import_item("maxi-lens",48,{"camera-stand","camera-cover"},"Camera zoom lens"), |
| import_item(" | ipac-laptop | ", | 49.0 | ,{" | black-computer | "," | white-monitor | "}," | I-Pac Laptop | "), | import_item("ipac-laptop",49,{"black-computer","white-monitor"},"I-Pac Laptop"), |
| import_item(" | balcony-laptop | ", | 50.0 | ,{" | white-computer | "," | black-monitor | "}," | Balcony 7 Laptop | "), | import_item("balcony-laptop",50,{"white-computer","black-monitor"},"Balcony 7 Laptop"), |
| import_item(" | low-tech-monitor | ", | 51.0 | ,{" | cheap-monitor | "," | wide-monitor | "}," | Brickview CRT Monitor | "), | import_item("low-tech-monitor",51,{"cheap-monitor","wide-monitor"},"Brickview CRT Monitor"), |
| import_item(" | cheap-monitor | ", | 52.0 | ,{" | low-tech-monitor | "," | wide-monitor | "}," | 4x4 Monitor (black) | "), | import_item("cheap-monitor",52,{"low-tech-monitor","wide-monitor"},"4x4 Monitor (black)"), |
| import_item(" | wide-monitor | ", | 53.0 | ,{" | low-tech-monitor | "," | cheap-monitor | "}," | 8x4 Monitor (black) | "), | import_item("wide-monitor",53,{"low-tech-monitor","cheap-monitor"},"8x4 Monitor (black)"), |
| import_item(" | black-computer | ", | 54.0 | ,{" | white-computer | "," | wide-monitor | "}," | Computer case (black) | "), | import_item("black-computer",54,{"white-computer","wide-monitor"},"Computer case (black)"), |
| import_item(" | white-computer | ", | 55.0 | ,{" | black-computer | "," | low-tech-monitor | "}," | Computer case (white) | "), | import_item("white-computer",55,{"black-computer","low-tech-monitor"},"Computer case (white)"), |
| import_item(" | black-keyboard | ", | 56.0 | ,{" | white-keyboard | "," | black-mouse | "}," | Keyboard (black) | "), | import_item("black-keyboard",56,{"white-keyboard","black-mouse"},"Keyboard (black)"), |
| import_item(" | white-keyboard | ", | 57.0 | ,{" | black-keyboard | "," | white-mouse | "}," | Keyboard (white) | "), | import_item("white-keyboard",57,{"black-keyboard","white-mouse"},"Keyboard (white)"), |
| import_item(" | black-mouse | ", | 58.0 | ,{" | white-mouse | "," | black-keyboard | "}," | Mouse (black) | "), | import_item("black-mouse",58,{"white-mouse","black-keyboard"},"Mouse (black)"), |
| import_item(" | white-mouse | ", | 59.0 | ,{" | black-mouse | "," | white-keyboard | "}," | Mouse (white) | "), | import_item("white-mouse",59,{"black-mouse","white-keyboard"},"Mouse (white)"), |
| import_item(" | tablet | ", | 60.0 | ,{" | phone-flip | "," | phone-robust | "}," | Tablet (black) | "), | import_item("tablet",60,{"phone-flip","phone-robust"},"Tablet (black)"), |
| import_item(" | phone-robust | ", | 62.0 | ,{" | phone-one-button | "," | phone-touch | "}," | Nokeys Robust Telephony device | "), | import_item("phone-robust",62,{"phone-one-button","phone-touch"},"Nokeys Robust Telephony device"), |
| import_item(" | phone-simple | ", | 63.0 | ,{" | phone-one-button | "," | phone-touch | "}," | ErikGrunnson Simple phone | "), | import_item("phone-simple",63,{"phone-one-button","phone-touch"},"ErikGrunnson Simple phone"), |
| import_item(" | phone-flip | ", | 64.0 | ,{" | phone-one-button | "," | phone-touch | "}," | RazorSharp Flip phone | "), | import_item("phone-flip",64,{"phone-one-button","phone-touch"},"RazorSharp Flip phone"), |
| import_item(" | phone-touch | ", | 65.0 | ,{" | phone-robust | "," | phone-simple | "}," | OneScreen Touch phone | "), | import_item("phone-touch",65,{"phone-robust","phone-simple"},"OneScreen Touch phone"), |
| import_item(" | music-player | ", | 66.0 | ,{" | phone-flip | "," | phone-robust | "}," | I-Pac music player | "), | import_item("music-player",66,{"phone-flip","phone-robust"},"I-Pac music player"), |
| import_item(" | phone-touch-button | ", | 67.0 | ,{" | phone-robust | "," | phone-simple | "}," | OneButton Touch phone | "), | import_item("phone-touch-button",67,{"phone-robust","phone-simple"},"OneButton Touch phone"), |
| import_item(" | tape-player | ", | 68.0 | ,{" | tape-measure | "," | white-keyboard | "}," | Cassette player | "), | import_item("tape-player",68,{"tape-measure","white-keyboard"},"Cassette player"), |
| import_item(" | reader-white | ", | 69.0 | ,{" | reader-green | "," | phone-robust | "}," | E-Reader - ultra white - backlit | "), | import_item("reader-white",69,{"reader-green","phone-robust"},"E-Reader - ultra white - backlit"), |
| import_item(" | reader-green | ", | 71.0 | ,{" | reader-white | "," | phone-robust | "}," | E-Reader - nightvision - green | "), | import_item("reader-green",71,{"reader-white","phone-robust"},"E-Reader - nightvision - green"), |
| import_item(" | hand-calculator | ", | 72.0 | ,{" | desk-calculator | "," | tape-player | "}," | Handheld calculator | "), | import_item("hand-calculator",72,{"desk-calculator","tape-player"},"Handheld calculator"), |
| import_item(" | usb-stick | ", | 73.0 | ,{" | ram-stick | "," | tape-player | "}," | USB stick (128tb) | "), | import_item("usb-stick",73,{"ram-stick","tape-player"},"USB stick (128tb)"), |
| import_item(" | desk-calculator | ", | 74.0 | ,{" | hand-calculator | "," | tape-player | "}," | Desk calculator | "), | import_item("desk-calculator",74,{"hand-calculator","tape-player"},"Desk calculator"), |
| import_item(" | motherboard | ", | 75.0 | ,{" | ram-stick | "," | cheap-monitor | "}," | Motherboard - 3 slots | "), | import_item("motherboard",75,{"ram-stick","cheap-monitor"},"Motherboard - 3 slots"), |
| import_item(" | ram-stick | ", | 76.0 | ,{" | motherboard | "," | usb-stick | "}," | Ram stick - 3 chips | "), | import_item("ram-stick",76,{"motherboard","usb-stick"},"Ram stick - 3 chips"), |
| import_item(" | cheap-gpu | ", | 77.0 | ,{" | ram-stick | "," | hand-calculator | "}," | Budget++ Graphics card | "), | import_item("cheap-gpu",77,{"ram-stick","hand-calculator"},"Budget++ Graphics card"), |
| import_item(" | fast-gpu | ", | 78.0 | ,{" | motherboard | "," | desk-calculator | "}," | Mega++ Graphic card | "), | import_item("fast-gpu",78,{"motherboard","desk-calculator"},"Mega++ Graphic card"), |
| import_item(" | stick-flight | ", | 79.0 | ,{" | stick-retro | "," | ram-stick | "}," | Joystick - Flightmagic | "), | import_item("stick-flight",79,{"stick-retro","ram-stick"},"Joystick - Flightmagic"), |
| import_item(" | stick-retro | ", | 80.0 | ,{" | stick-flight | "," | controller-retro | "}," | Joystick - Retro | "), | import_item("stick-retro",80,{"stick-flight","controller-retro"},"Joystick - Retro"), |
| import_item(" | controller-retro | ", | 81.0 | ,{" | controller-next-gen | "," | stick-retro | "}," | Game controller - retro | "), | import_item("controller-retro",81,{"controller-next-gen","stick-retro"},"Game controller - retro"), |
| import_item(" | controller-next-gen | ", | 82.0 | ,{" | controller-retro | "," | fast-gpu | "}," | Game controller - next gen | "), | import_item("controller-next-gen",82,{"controller-retro","fast-gpu"},"Game controller - next gen"), |
| import_item(" | microphone | ", | 83.0 | ,{" | headphones | "," | scope-micro | "}," | Microphone | "), | import_item("microphone",83,{"headphones","scope-micro"},"Microphone"), |
| import_item(" | headphones | ", | 84.0 | ,{" | microphone | "," | scope-heart | "}," | Headphone | "), | import_item("headphones",84,{"microphone","scope-heart"},"Headphone"), |
| import_item(" | syringe | ", | 93.0 | ,{" | thermometer | "," | toothbrush | "}," | Injector 46hundred - syringe | "), | import_item("syringe",93,{"thermometer","toothbrush"},"Injector 46hundred - syringe"), |
| import_item(" | thermometer | ", | 94.0 | ,{" | syringe | "," | toothbrush | "}," | Tempmaster 4600 - thermometer | "), | import_item("thermometer",94,{"syringe","toothbrush"},"Tempmaster 4600 - thermometer"), |
| import_item(" | toothbrush | ", | 95.0 | ,{" | thermometer | "," | syringe | "}," | GeneriCo toothbrush | "), | import_item("toothbrush",95,{"thermometer","syringe"},"GeneriCo toothbrush"), |
| import_item(" | pills | ", | 99.0 | ,{" | band-aid | "," | first-aid | "}," | GrowingPains Painkillers (24 pack) | "), | import_item("pills",99,{"band-aid","first-aid"},"GrowingPains Painkillers (24 pack)"), |
| import_item(" | band-aid | ", | 100.0 | ,{" | first-aid | "," | pills | "}," | Adhesive fix - single unit | "), | import_item("band-aid",100,{"first-aid","pills"},"Adhesive fix - single unit"), |
| import_item(" | first-aid | ", | 102.0 | ,{" | band-aid | "," | pills | "}," | First-aid kit | "), | import_item("first-aid",102,{"band-aid","pills"},"First-aid kit"), |
| import_item(" | iodine | ", | 103.0 | ,{" | nail-polish | "," | pills | "}," | Iodine - bottled - 200ml | "), | import_item("iodine",103,{"nail-polish","pills"},"Iodine - bottled - 200ml"), |
| import_item(" | nail-polish | ", | 104.0 | ,{" | iodine | "," | thermometer | "}," | Nail polish - 100ml | "), | import_item("nail-polish",104,{"iodine","thermometer"},"Nail polish - 100ml"), |
| import_item(" | scope-heart | ", | 110.0 | ,{" | scope-micro | "," | thermometer | "}," | Stethoscope | "), | import_item("scope-heart",110,{"scope-micro","thermometer"},"Stethoscope"), |
| import_item(" | scope-micro | ", | 111.0 | ,{" | scope-heart | "," | microphone | "}," | Microscope | "), | import_item("scope-micro",111,{"scope-heart","microphone"},"Microscope"), |
