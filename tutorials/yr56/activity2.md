# Multiple Upgrades

```template
let cookies = 0
let grandmas = 0
let farms = 0
let grandmaCost = 15
let farmCost = 100
let cookiesPerSecond = 0
scene.setBackgroundImage(img`bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbfffffffffffffffffbbfffffffffbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbf999999996999999fbbf6999999fbbbbbbbfffffffffbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbf6999999966999999fbf6999999fbbbbbbbbf6999999fbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbffffffffbbbbbbbbbbbbbbbbbf999999996999999ffbf6999999fbbbbbbbff699999fbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbffffffffbbbbfe44444fbbbbbbbbbbbbbbbbf6999999966999999fbf6999999fbbbbbbbbf6999999fbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbffffffffffffffbbbbbbbbbbbbbbbbbbbbbbbbbbfe44444fbbbbfe44444fbbbbbbbbbbbbbbbbf999966666999999ffbf666666bfbbbbbbbbf6999999fbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbfe44444444444fbbbbbbbbbbbbbbbbbbbbbbbbbbfe44444fbbbbfeeeeeefbbbbbbbbbbbbbbbf6999fffff6999999fbbffffffffbbbbbbbbbf699999fbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbfe44444444444fbbbbbbbbbbbbbbbbbbbbbbbbbbfe44444fbbbbffffffffbbbbbbbbbbbbbbbf6999fbbbf699999fbbfffffffffffffffffff699999fbbffffffffffffffffffffffffffffbbb
bbbbbbfe44444444444ffffffffffffffffffffffffffffe44444fbbfffffffffffffffffffffbbbf6999fbbbf6999999fbbf69999669999999996699999fbbf996699999999996699999999999fbbb
bbbbbbfe44444444444fe444444444444e4444444444444e44444fbf444e44444e4444444444fbbbf6999fbbbf699999fbbbf69999669999999996699999fbf9996699999999996699999999999fbbb
bbbbbbfe44444444444fe444444444444e4444444444444e44444ff4444e44444e4444444444fbbf69999fbbbf699999fbbf699996699999999966699999ff9996699999999999699999999999fbbbb
bbbbbbfe4444eeeeeeefe444444444444e4444444444444e44444ff4444e44444e4444444444fbbf6999fbbbf6999999fbbf69999669999999996669999ff99996699999999996699996666999fbbbb
bbbbbbfe4444ffffffffe444eeeeeee44e444eeeeeee444e44444f4444ee44444e4444444444fbbf9999fbbbf699999fbbbf99996699999999996699999f99996669999999999669999fff6999fbbbb
bbbbbbfe4444fbbbbbbfe444ffffffe44e444ffffffe444e4444444444ee44444e444eeeeeeefbf69999fbbf6999999fbbf69999669999ffffff669999999999f69999996666666999fbbf9999fbbbb
bbbbbbfe4444fbbbbbbfe444fbbbbfe44e444fbbbbfe444e444444444efe44444e444ffffffffbf6999fbbbf699999fbbbf69999669999fbbbbf66999999999666999999fffff69999fbf6999fbbbbb
bbbbbbfe4444fbbbbbbfe444fbbbbfe44e444fbbbbfe444e444444444efe44444e44444444fbbf69999fbbbf699999fbbf69999669999fbbbbff69999999996f6699999ffffff69999fff6999fbbbbb
bbbbbbfe4444fbbbbbbfe444fbbbbfe44e444fbbbbfe444e44444444effe44444e44444444fbbf6999fbbbf6999999fbbf69999669999fbbbbf66999999996ff699999999999f699999999999fbbbbb
bbbbbbfe4444ffffffffe444fbbbbfe44e444fbbbbfe444e444444444ffe44444e444eeeeefbf69999fbbbf699999fbbbf69999669999fbbbbf6699999999ff669999999999ff999999999999fbbbbb
bbbbbbfe444444444444e444ffffffe44e444ffffffe444e44444e4444fe44444e444ffffffbf69999fbbbf699999fbbf699996699999fbbbbf66999999999f699999999999f699999999999fbbbbbb
bbbbbbfe444444444444e444444444444e4444444444444e44444fe4444e44444e444fffffff66999fbbbf699999fbbbf69999669999fbbbbf6699999699996699999666666f699999999999fbbbbbb
bbbbbbfe444444444444e444444444444e4444444444444e44444ffe444e44444e44444444ef69999fffff699999ffff699996699999ffffff6699999f69996699999ffffff6999999666666fbbbbbb
bbbbbbfe444444444444e444444444444e4444444444444e44444fbf444e44444e4444444ef6699999996699999999966999966999999999996699999ff996699999fffffff6999999999ffffbbbbbb
bbbbbbfeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeeefbfeeeeeeeeeeeeeeeeeef6999999996699999999966999966999999999996699999ff69669999999999966999969999fbbbbbbbbb
bbbbbbffffffffffffffffffffffffffffffffffffffffffffffffbbfffffffffffffffffff699999996669999999966999966999999999996699999fbbf96699999999996669999f69999fbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbf6699999996699999999966999966999999999996699999fbbbf6999999999996699999ff6999fbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbf6666666666666666666666666666666666666666666666fbbbf6666666666666666666fbf6666fbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbffffffffffffffffffffffffffffffffffffffffffffffffbbbbffffffffffffffffffffbbfffffbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbcbdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbccbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbddddddddddddddddddddddddddddbbbbbbbbbcdddddddddddddddddddddddddddbbbbbbbbb
bbcbdcccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbddddddddddddddddddddddddddddddbbbbbbbcdddddddddddddddddddddddddddddbbbbbbbb
bbcbdcccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbdddddddddddddddddddddddddddddddbbbbbbcddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbbccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbdddddddddddddddddddddddddddddddbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbbddddddddddddddddddddddddddddddbbbbccccdddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbcccccccccccccccccccccccccccccccbbbbcccccccccccccccccccccccccccccccccbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbcccccccccccccccccccccccccccccccbbbbbccccccccccccccccccccccccccccccccbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbcccccccccccccccccccccccccccccccbbbbbbbccccccccccccccccccccccccccccccbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbdddddddddddddddddddddddddddbbbbbbbbbbcdddddddddddddddddddddddddddbbbbbbbbb
bbcbdcccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbdddddddddddddddddddddddddddddbbbbbbbbcdddddddddddddddddddddddddddddbbbbbbbb
bbcbdcccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbddddddddddddddddddddddddddddddbbbbbbbcddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbbccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbddddddddddddddddddddddddddddddbbbbbcccddddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbbdddddddddddddddddddddddddddddbbbbbccccdddddddddddddddddddddddddddddbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbccccccccccccccccccccccccccccccbbbbbcccccccccccccccccccccccccccccccccbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbccccccccccccccccccccccccccccccbbbbbbccccccccccccccccccccccccccccccccbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbccccccccccccccccccccccccccccccbbbbbbbbccccccccccccccccccccccccccccccbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbdbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbdddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddddbcbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbcbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbccbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccccbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb
bbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbbb`)

let cookie = sprites.create(img`
...............................
............dddddd.............
.........44444444444d..........
.......e44444ed44dd444d........
......e444444eee4444444d.......
....e44444444eee44444d44dd.....
....4444edd444e4444444444d.....
...e444eeed444444444444444d....
..e4444eeee444444dd444e4d4dd...
..444444eee44444eed44eee444d...
.e444444ee444444ee444eee4444d..
.e44444444444444444444ee44444..
e44ee444444444444444444444444..
e44ee44444444ed44444444444444d.
e444444444444eee4444444dd4444d.
e444444444444ee4444444eedd444d.
e444444e4444444444d444eeee444d.
e44444eee44444444edd44eee4444d.
ee4444eeee44eed44eee44444444dd.
.e44444ee444eee44ee44444e444d..
.ee44444e444eee44444444eeee44..
.ee4444444444ee44444444eee44d..
..e444444444444444444444e444...
..ee444444e44444444444444444...
...e44444eee444eee444444444....
....ee444eee444eee444eed44.....
.....ee444e4444eee44eeee4e.....
......eee4444444e4444eee.......
........eee4444444444ee........
.........eeeee44444ee..........
............eeeeee.............
...............................
`, SpriteKind.Player)
cookie.setPosition(45, 75)
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += 1
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= grandmaCost) {
        cookies -= grandmaCost
        grandmas += 1
        cookiesPerSecond += 1
        grandmaCost = Math.round(grandmaCost * 1.15)
        info.setScore(cookies)
    } else {
        game.showLongText("Grandma costs " + grandmaCost + " cookies!", DialogLayout.Bottom)
    }
})
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= farmCost) {
        cookies -= farmCost
        farms += 1
        cookiesPerSecond += 8
        farmCost = Math.round(farmCost * 1.15)
        info.setScore(cookies)
    } else {
        game.showLongText("Farm costs " + farmCost + " cookies!", DialogLayout.Bottom)
    }
})
game.onUpdateInterval(1000, function () {
    if (cookiesPerSecond > 0) {
        cookies += cookiesPerSecond
        info.setScore(cookies)
    }
})
```

## What are Multiple Alternatives? @showdialog

Your shop from Activity 1 is already loaded — you can see the cookie, score, and two working upgrades (Grandma and Farm)!

In Activity 1 you used a simple ``if/else`` — two choices. But real programs often need to handle **many different situations**.

In code, ``else if`` lets you chain multiple conditions together:

```
if condition1 then ...
else if condition2 then ...
else if condition3 then ...
else ... (none of the above)
```

In this activity you will:
- Add a **Factory** as a third upgrade
- Replace simple if/else with ``else if`` chains that give players useful feedback
- Add a **combined condition** using ``AND`` — multiple things must be true at the same time


## Step 1 — Add Factory variables

In ``||loops:on start||``, add two new variables:
- ``factories`` starting at **0**
- ``factoryCost`` starting at **500**

```blockconfig.local
let factories = 0
let factoryCost = 500
```

```blocks
let cookies = 0
let grandmas = 0
let farms = 0
let factories = 0
let grandmaCost = 15
let farmCost = 100
let factoryCost = 500
let cookiesPerSecond = 0
```

## Step 2 — Buy a Factory (Down button)

Add a ``||controller:on down button pressed||`` event.

Use a simple ``if/else`` first (you will upgrade it in the next step):
- If ``cookies >= factoryCost``: buy the factory (adds **47** cookiesPerSecond), multiply cost by 1.15
- Else: show cost message

```blocks
controller.down.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= factoryCost) {
        cookies -= factoryCost
        factories += 1
        cookiesPerSecond += 47
        factoryCost = Math.round(factoryCost * 1.15)
        info.setScore(cookies)
    } else {
        game.showLongText("Factory costs " + factoryCost + " cookies!", DialogLayout.Bottom)
    }
})
```

## Step 3 — Multiple alternatives: upgrade the Grandma handler

Open your ``||controller:on B button pressed||`` (Grandma) event.

Right now it only has two outcomes (can afford / cannot afford). Let's add a **helpful middle message** using ``else if``.

Replace the current ``else`` with an ``else if`` that checks if the player is *close* to affording it (within 50% of the cost), and put a different message there:

- ``if cookies >= grandmaCost`` → buy grandma
- ``else if cookies >= grandmaCost / 2`` → "Almost there! Need X more cookies"
- ``else`` → "Keep baking! Grandma costs X cookies"

To add ``else if``: click the **+** button at the bottom of your ``||logic:if||`` block.

```blockconfig.local
if (cookies >= grandmaCost) {
} else if (cookies >= grandmaCost / 2) {
} else {
}
```

```blocks
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= grandmaCost) {
        cookies -= grandmaCost
        grandmas += 1
        cookiesPerSecond += 1
        grandmaCost = Math.round(grandmaCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= grandmaCost / 2) {
        game.showLongText("Almost there! Need " + (grandmaCost - cookies) + " more cookies.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Grandma costs " + grandmaCost + " cookies.", DialogLayout.Bottom)
    }
})
```

## Step 4 — Apply the same pattern to Farm and Factory

Update your ``||controller:on up button pressed||`` (Farm) event to also use three alternatives:

- If the player can afford → buy
- Within 50% → "Almost there! Need X more cookies"
- Otherwise → "Keep baking! Y costs X cookies"

Do the same for ``||controller:on down button pressed||`` (Factory).

**Notice the pattern:** The *shape* of the code is the same for all three upgrades, just the variable names change. This is called a **pattern** in algorithm design.

```blocks
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= farmCost) {
        cookies -= farmCost
        farms += 1
        cookiesPerSecond += 8
        farmCost = Math.round(farmCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= farmCost / 2) {
        game.showLongText("Almost there! Need " + (farmCost - cookies) + " more for a Farm.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Farm costs " + farmCost + " cookies.", DialogLayout.Bottom)
    }
})
```

## Step 5 — Combined condition: AND logic

What if we want to give a player a **bonus** when they have BOTH grandmas AND farms?

In the ``||game:on game update every 1000 ms||`` block, add a check using ``||logic:and||``:

**if grandmas >= 5 AND farms >= 3** → add an extra **10 cookies** bonus per second (on top of normal production).

```blockconfig.local
if (grandmas >= 5 && farms >= 3) {
    cookies += 10
    info.setScore(cookies)
}
```

```blocks
game.onUpdateInterval(1000, function () {
    if (cookiesPerSecond > 0) {
        cookies += cookiesPerSecond
        info.setScore(cookies)
    }
    if (grandmas >= 5 && farms >= 3) {
        cookies += 10
        info.setScore(cookies)
    }
})
```

## Step 6 — Test all three upgrade paths

Test the game and verify each path works:

1. Press B when you have 0 cookies — see the "keep baking" message
2. Bake 8 cookies — press B and see the "almost there" message  
3. Bake 15 cookies — press B and buy a grandma
4. Bake 100 cookies — press Up for a farm
5. Build 5 grandmas and 3 farms — watch for the bonus!

**Think about it:** Count how many different paths your program can take in just the B button event. (Answer: 3 paths, one per condition!)

## Challenge: Add an OR condition

Can you add a bonus that triggers if the player has **either** 10 grandmas **OR** 5 farms? Find the ``||logic:or||`` block and add it to the update loop!

## Multiple alternatives mastered! @showdialog

**Brilliant work!** You have moved beyond simple if/else to proper multiple-alternative branching.

**What you built:**
- Three upgrade types with different costs and production rates
- ``else if`` chains giving players 3 different responses
- A combined condition using ``AND`` for a synergy bonus

**What this means (AC9TDI6P02):** You designed and implemented algorithms with *multiple alternatives* — your program takes many different paths depending on several conditions.

**Next up:** Activity 3 — you will use **for loops** to calculate your production more efficiently!
