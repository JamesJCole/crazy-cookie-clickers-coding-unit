# Adding Controls

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

## How are players meant to play the game? @showdialog

Players have the ability to do the following:
- Bake Individual Cookies
- Purchase a Grandma
- Purchase a Farm
- Purchase a Factory

Each of these things have a different control that they are mapped to.
We need to make those controls visible to the player.


## Step 1 - Make a 'Bake' button
First, we need a 'bake' button  for individual 'cookies'. To do this, we will want to do the following:
1. Setup a 'sprite' for the AButton. ``||sprites:set AButton to sprite of kind Player||`` 
2. Now position the 'AButton' on the screen (recommended: *x:100, y:49*)

You can replace the 'example' components with your own versions!

We are going to repeat this for the next few 'steps'.

```blockconfig.local
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

```

```blocks
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
AButton.setPosition(100, 49)
```
## Step 1.5 - Make a Label for Bake Button
Next we need a label for our 'bake' button. To do this, we will want to do the following:
1. Create a 'sprite' for the BakeLabel.  ``||sprites:set BakeLabel to sprite of kind Player||`` 
2. Now position the 'BakeLabel' on the screen (recommended: *x:100, y:60*)

You can replace the 'example' components with your own versions!

```blockconfig.local
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
```

```blocks
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
BakeLabel.setPosition(100, 60)
```
## Step 2 - Make a 'Grandma' Button
Second, we need a 'Grandma' button  for individual 'Grandmas'. To do this, we will want to do the following:
1. Setup a 'sprite' for the UpButton. ``||sprites:set UpButton to sprite of kind Player||`` 
3. Now position the 'UpButton' on the screen (recommended: *x:100, y:49*)


```blockconfig.local
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

```

```blocks
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
    

UpButton.setPosition(100, 49)
```
## Step 2.5 - Make a Label for the 'Grandma' Button
Now we will want a label for the up button we are using to 'create' 'Grandma's'
1. Create a 'sprite' for the GrandmaLabel.  ``||sprites:set GrandmaLabel to sprite of kind Player||`` 
2. Now position the 'GrandmaLabel' on the screen (recommended: *x:100, y:60*)


```blockconfig.local
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

```

```blocks
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

GrandmaLabel.setPosition(100, 60)
```

## Step 3 - Make a 'Farm' Button
Lets repeat for the Farm Button
1. Setup a 'sprite' for the RightButton. ``||sprites:set RightButton to sprite of kind Player||`` 
2. Now position the 'RightButton' on the screen (recommended: *x:100, y:49*)


```blockconfig.local
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

```

```blocks
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
    


RightButton.setPosition(100, 49)
```
## Step 3.5 - Farm Label
Now the farm label:
1. Create a 'sprite' for the FarmLabel.  ``||sprites:set FarmLabel to sprite of kind Player||`` 
2. Now position the 'FarmLabel' on the screen (recommended: *x:100, y:60*)


```blockconfig.local
    
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

```

```blocks

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

FarmLabel.setPosition(100, 60)
```


## Step 4 - Make a 'Factory' Button
Lastly, the 'Factory' button:
1. Setup a 'sprite' for the LeftButton. ``||sprites:set LeftButton to sprite of kind Player||``
3. Now position the 'LeftButton' on the screen (recommended: *x:100, y:49*)


```blockconfig.local
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
    

```

```blocks
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
    

LeftButton.setPosition(100, 49)
```
## Step 4.5 - Factory Label
Now the Factory Label:
1. Create a 'sprite' for the GrandmaLabel.  ``||sprites:set  FactoryLabel to sprite of kind Player||`` 
2. Now position the 'FactoryLabel' on the screen (recommended: *x:100, y:60*)


```blockconfig.local
    
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

```

```blocks
    
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

FactoryLabel.setPosition(100, 60)
```

## Step 5 - Testing
Now try testing the game and make sure all the labels show.
Try changing or updating the sprites with your own creations!
