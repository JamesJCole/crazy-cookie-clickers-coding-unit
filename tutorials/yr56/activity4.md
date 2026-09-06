# Cookie Multipliers

```template
let cookies = 0
let grandmas = 0
let farms = 0
let factories = 0
let grandmaCost = 15
let farmCost = 100
let factoryCost = 500
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
let AButton = sprites.create(img`
    . . . . . . . . . . . . . . . 
    . . . . . 7 7 7 1 1 . . . . . 
    . . . . 7 7 7 7 7 7 7 1 . . . 
    . . 6 7 7 7 7 7 7 7 7 7 1 . . 
    . 6 7 7 7 7 7 6 6 7 7 7 7 . . 
    . 6 7 7 7 7 6 7 7 6 7 7 7 1 . 
    6 6 7 7 7 7 6 6 6 6 7 7 7 7 . 
    6 6 7 7 7 7 6 7 7 6 7 7 7 7 . 
    6 6 7 7 7 7 6 7 7 6 7 7 7 7 . 
    6 6 7 7 7 7 7 7 7 7 7 7 7 7 . 
    . 6 6 7 7 7 7 7 7 7 7 7 7 . . 
    . 6 6 6 7 7 7 7 7 7 7 7 6 . . 
    . . 6 6 6 7 7 7 7 7 6 6 . . . 
    . . . 6 6 6 6 6 6 6 6 . . . . 
    . . . . 6 6 6 6 6 . . . . . . 
    . . . . . . . . . . . . . . . 
    `, SpriteKind.Player)

let BakeLabel = sprites.create(img`
    . . f f f f f f f f f f f f f f f f f f f f f f f . . 
    . f 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 f . 
    f 1 1 f f f 1 1 1 f f 1 1 f 1 1 f 1 f f f 1 1 f 1 1 f 
    f 1 1 f 1 1 f 1 f 1 1 f 1 f 1 f 1 1 f 1 1 1 1 f 1 1 f 
    f 1 1 f f f 1 1 f f f f 1 f f 1 1 1 f f f 1 1 f 1 1 f 
    f 1 1 f 1 1 f 1 f 1 1 f 1 f 1 f 1 1 f 1 1 1 1 1 1 1 f 
    f 1 1 f f f f 1 f 1 1 f 1 f 1 1 f 1 f f f 1 1 f 1 1 f 
    . f 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 1 f . 
    . . f f f f f f f f f f f f f f f f f f f f f f f . . 
    `, SpriteKind.Player)

let UpButton = sprites.create(img`
    . . . . . . 5 5 5 . . . . . . 
    . . . . . 4 4 4 4 4 . . . . . 
    . . . . . . . . . . . . . . . 
    . . . . . 6 9 9 1 1 . . . . . 
    . . . . . 6 9 9 9 9 . . . . . 
    . . . . . 6 9 9 9 9 . . . . . 
    . . . . . 6 9 9 9 9 . . . . . 
    . 6 9 1 1 9 9 9 9 9 1 1 1 1 . 
    . 6 9 9 9 9 9 9 9 9 9 9 9 9 . 
    . 6 9 9 9 9 9 9 9 9 9 9 9 9 . 
    . 6 9 9 9 9 9 9 9 9 9 9 9 9 . 
    . . 6 6 6 6 9 9 9 1 6 6 6 6 . 
    . . . . . 6 9 9 9 1 . . . . . 
    . . . . . 6 9 9 9 1 . . . . . 
    . . . . . 6 9 9 9 9 . . . . . 
    . . . . . 6 6 6 6 6 . . . . . 
    `, SpriteKind.Player)

let GrandmaLabel = sprites.create(img`
    ..ffffffffffffffffffffffffffffffffffffff..
    .f11111111111111111111111111111111111111f.
    f11fff11ffff11ff11ff11fff11ff1ff11ff11f11f
    f11f1111f11f1f11f1f1f1f11f1f1f1f1f11f1f11f
    f11f1ff1ffff1ffff1f1f1f11f1f111f1ffff1f11f
    f11f11f1f1f11f11f1f1f1f11f1f111f1f11f1111f
    f11ffff1f11f1f11f1f1f1fff11f111f1f11f1f11f
    .f11111111111111111111111111111111111111f.
    ..ffffffffffffffffffffffffffffffffffffff..
`, SpriteKind.Player)

let RightButton = sprites.create(img`
    . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . 
    . . . 6 9 9 1 1 . . . . . . . 
    . . . 6 9 9 9 9 . . . . . . . 
    . . . 6 9 9 9 9 . . . . . . . 
    . . . 6 9 9 9 9 . . . . . . . 
    9 1 1 9 9 9 9 9 1 1 1 1 . 4 . 
    9 9 9 9 9 9 9 9 9 9 9 9 . 4 5 
    9 9 9 9 9 9 9 9 9 9 9 9 . 4 5 
    9 9 9 9 9 9 9 9 9 9 9 9 . 4 5 
    6 6 6 6 9 9 9 1 6 6 6 6 . 4 . 
    . . . 6 9 9 9 1 . . . . . . . 
    . . . 6 9 9 9 1 . . . . . . . 
    . . . 6 9 9 9 9 . . . . . . . 
    . . . 6 6 6 6 6 . . . . . . . 
    . . . . . . . . . . . . . . . 
    `, SpriteKind.Player)
    

let FarmLabel = sprites.create(img`
    ..fffffffffffffffffffffff..
    .f11111111111111111111111f.
    f11fff11ff11ffff1ff1ff1f11f
    f11f111f11f1f11f1f1f1f1f11f
    f11fff1ffff1ffff1f111f1f11f
    f11f111f11f1f1f11f111f1111f
    f11f111f11f1f11f1f111f1f11f
    .f11111111111111111111111f.
    ..fffffffffffffffffffffff..
`, SpriteKind.Player)

let LeftButton = sprites.create(img`
    ................
    ................
    .......69911....
    .......69999....
    .......69999....
    .......69999....
    .4.6911999991111
    54.6999999999999
    54.6999999999999
    54.6999999999999
    .4..666699916666
    .......69991....
    .......69991....
    .......69999....
    .......66666....
    ................
`, SpriteKind.Player)

let FactoryLabel = sprites.create(img`
    ..ffffffffffffffffffffffffffffffffff..
    .f1111111111111111111111111111111111f.
    f11fff11ff11fff1fff1ffff1ffff1f1f1f11f
    f11f111f11f1f1111f11f11f1f11f1f1f1f11f
    f11fff1ffff1f1111f11f11f1ffff11f11f11f
    f11f111f11f1f1111f11f11f1f1f111f11111f
    f11f111f11f1fff11f11ffff1f11f11f11f11f
    .f1111111111111111111111111111111111f.
    ..ffffffffffffffffffffffffffffffffff..
`, SpriteKind.Player)

BakeLabel.setPosition(100, 62)
AButton.setPosition(100, 51)
UpButton.setPosition(136, 51)
GrandmaLabel.setPosition(136, 62)
RightButton.setPosition(100, 90)
FarmLabel.setPosition(100, 1000)
LeftButton.setPosition(136, 90)
FactoryLabel.setPosition(136, 100)
cookie.setPosition(45, 75)
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += 1
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= grandmaCost) {
        cookies -= grandmaCost
        grandmas += 1
        grandmaCost = Math.round(grandmaCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= grandmaCost / 2) {
        game.showLongText("Almost there! Need " + (grandmaCost - cookies) + " more cookies.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Grandma costs " + grandmaCost + " cookies.", DialogLayout.Bottom)
    }
})
controller.right.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= farmCost) {
        cookies -= farmCost
        farms += 1
        farmCost = Math.round(farmCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= farmCost / 2) {
        game.showLongText("Almost there! Need " + (farmCost - cookies) + " more for a Farm.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Farm costs " + farmCost + " cookies.", DialogLayout.Bottom)
    }
})
controller.left.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= factoryCost) {
        cookies -= factoryCost
        factories += 1
        factoryCost = Math.round(factoryCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= factoryCost / 2) {
        game.showLongText("Almost there! Need " + (factoryCost - cookies) + " more for a Factory.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Factory costs " + factoryCost + " cookies.", DialogLayout.Bottom)
    }
})
game.onUpdateInterval(1000, function () {
    let total = 0
    for (let i = 0; i <= 2; i++) {
        if (i == 0) {
            total += grandmas * 1
        } else if (i == 1) {
            total += farms * 8
        } else if (i == 2) {
            total += factories * 47
        }
    }
    cookiesPerSecond = total
    cookies += cookiesPerSecond
    info.setScore(cookies)
    if (grandmas >= 5 && farms >= 3) {
        cookies += 10
    }
})
```

## Nested Conditions @showdialog

Your factory from Activities 1–3 is already loaded — three upgrades, ``else if`` messages, and a for loop calculating production each second!

So far your conditions are fairly straightforward. But what about a situation where you need to check **one thing, and then another thing depending on the first result**?

That is **nested conditions** — an ``if`` block inside another ``if`` block:

```
if grandmas >= 10 then
    if farms >= 5 then
        bonus = HUGE   (both grandmas AND farms maxed)
    else
        bonus = medium  (only grandmas)
else
    if farms >= 5 then
        bonus = medium  (only farms)
    else
        bonus = none    (neither)
```

In this activity you will:
- **Design** a bonus multiplier system on paper first
- **Implement** it using nested if/else
- Combine it with the for loop to apply the multiplier to total production

This is the most complex concept in this skillmap — take your time and think carefully!

This is **AC9TDI6P02** at its full depth.

## Step 1 — Design on paper first

**Algorithm design challenge — do this before touching code!**

Draw a flowchart (or write pseudocode) for this rule:

> Calculate a ``bonusMultiplier`` based on how many grandmas and farms you have:
> - grandmas ≥ 10 **AND** farms ≥ 5 → multiplier = **4** (master baker!)
> - grandmas ≥ 10 (but not enough farms) → multiplier = **2**
> - farms ≥ 5 (but not enough grandmas) → multiplier = **2**
> - neither condition met → multiplier = **1** (no bonus)

How many different outcomes are there? (Answer: 4)
How many conditions do you need to check? (Answer: 2, nested)

Show your design to your teacher before moving on.

## Step 2 — Create a bonusMultiplier variable

In ``||loops:on start||``, add a new variable ``bonusMultiplier`` and set it to **1**.

```blockconfig.local
let bonusMultiplier = 1
```

```blocks
let bonusMultiplier = 1
```

## Step 3 — The outer if (check grandmas)

After the for loop in your ``||game:on game update every 1000 ms||`` block, add the outer condition:

``if grandmas >= 10`` — this is the **outer** decision.

Inside the ``if``:
- Add another ``if/else`` to check ``farms >= 5``
- If farms also >= 5: set ``bonusMultiplier`` to **4**
- Else (grandmas >= 10 but not enough farms): set ``bonusMultiplier`` to **2**

```blockconfig.local
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
}
```

```blocks
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
}
```

## Step 4 — The outer else (grandmas < 10)

Add an ``else`` to the outer condition. Inside it:
- Add another ``if/else`` to check ``farms >= 5``
- If farms >= 5 (but grandmas < 10): set ``bonusMultiplier`` to **2**
- Else (neither): set ``bonusMultiplier`` to **1**

```blocks
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
} else {
    if (farms >= 5) {
        bonusMultiplier = 2
    } else {
        bonusMultiplier = 1
    }
}
```

## Step 5 — Apply the multiplier

Now use ``bonusMultiplier`` in your production calculation. Modify the for loop result:

After calculating ``total`` in the for loop, multiply by ``bonusMultiplier``:

```blockconfig.local
cookiesPerSecond = total * bonusMultiplier
```

```blocks
game.onUpdateInterval(1000, function () {
    let total = 0
    for (let i = 0; i <= 2; i++) {
        if (i == 0) {
            total += grandmas * 1
        } else if (i == 1) {
            total += farms * 8
        } else if (i == 2) {
            total += factories * 47
        }
    }
    if (grandmas >= 10) {
        if (farms >= 5) {
            bonusMultiplier = 4
        } else {
            bonusMultiplier = 2
        }
    } else {
        if (farms >= 5) {
            bonusMultiplier = 2
        } else {
            bonusMultiplier = 1
        }
    }
    cookiesPerSecond = total * bonusMultiplier
    cookies += cookiesPerSecond
    info.setScore(cookies)
})
```

## Step 6 — Test nested conditions

Verify each of the 4 outcomes:

1. **0 grandmas, 0 farms:** multiplier = 1 (no bonus) — check
2. **0 grandmas, 5+ farms:** multiplier = 2 — buy 5 farms and verify
3. **10+ grandmas, 0 farms:** multiplier = 2 — buy 10 grandmas and verify
4. **10+ grandmas, 5+ farms:** multiplier = 4 — build both and verify the CPS quadruples!

**Trace the nested logic:** For 10 grandmas and 3 farms, which path does the code take?
- Outer if: grandmas >= 10 ✓ → enter outer if
- Inner if: farms >= 5? No (3 < 5) → take inner else
- Result: multiplier = 2 ✓

## Step 7 — Refactor challenge

**Extension:** Can you refactor the nested condition into a *single* condition using ``AND`` and ``OR``?

Hint: ``if grandmas >= 10 AND farms >= 5`` for the 4× case, then two separate ``else if`` for the 2× cases.

Which approach is easier to read? Which is easier to extend? Discuss with a partner.

## Complex branching achieved! @showdialog

**Phenomenal work!** You have implemented one of the most complex patterns in programming.

**What you built:**
- A nested if/else system with 4 distinct outcomes
- A bonus multiplier applied through the production loop
- An algorithm you designed *before* implementing

**What this means (AC9TDI6P02):** You *designed* and implemented an algorithm with **complex branching** — nested conditions where the inner check depends on the outer result.

**Final activity:** Activity 5 — Cookie Empire. You will add a prestige system, a win condition, and put your complete game together!
