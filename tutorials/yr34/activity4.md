# Auto Baker

```template
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
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
cookie.setPosition(45, 70)
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
let UpgradeLabel = sprites.create(img`
    ..fffffffffffffffffffffffffffffffffffff..
    .f1111111111111111111111111111111111111f.
    f11f11f1ffff1fff11ffff11ff11fff11fff1f11f
    f11f11f1f11f1f1111f11f1f11f1f11f1f111f11f
    f11f11f1ffff1f1ff1ffff1ffff1f11f1fff1f11f
    f11f11f1f1111f11f1f1f11f11f1f11f1f111111f
    f11ffff1f1111ffff1f11f1f11f1fff11fff1f11f
    .f1111111111111111111111111111111111111f.
    ..fffffffffffffffffffffffffffffffffffff..
    `, SpriteKind.Player)
UpgradeLabel.setPosition(138, 60)
UpButton.setPosition(138, 49)
AButton.setPosition(100, 49)
BakeLabel.setPosition(100, 60)
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= upgradeCost) {
        cookies -= upgradeCost
        cookiesPerClick += 1
        info.setScore(cookies)
        music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
    } else {
        game.showLongText("Not enough cookies! Keep baking!", DialogLayout.Bottom)
    }
})
```

## What is Iteration? @showdialog

Your code from Activities 1–3 is already loaded — you have a clickable cookie and a working upgrade system!

Now let's take it to the next level: what if the game baked cookies **automatically**, without the player pressing anything?

Imagine a factory machine that stamps out cookies once every second, forever, without stopping.

That is **iteration** (also called a **loop**) — code that runs **again and again**, repeating its actions.

In this activity you will:
- Add an ``autoBakers`` variable to track your automatic bakers
- Add a button to buy an auto baker
- Use a ``||game:on game update every||`` block — a loop that runs every second
- Inside the loop, check **if** any auto bakers are working, then add cookies

This combines **branching** AND **iteration** — both from AC9TDI4P02!

## Step 1 — Add the autoBakers variable

In ``||loops:on start||``, create a new variable called ``autoBakers`` and set it to **0**.

Also add a variable ``autoBakerCost`` and set it to **50**.

```blockconfig.local
let autoBakers = 0
let autoBakerCost = 50
```

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
let autoBakers = 0
let autoBakerCost = 50
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
cookie.setPosition(80, 60)
info.setScore(0)
```

## Step 2 - Add a new button for 'auto baker'
We need to add the both an 'right' button 'sprite' and position it.
Find ``||sprites:set RightButton to sprite of kind Player||`` in the **Sprites** drawer. Drag it into ``||loops:on start||``.
Find ``||sprites:set RightButton position to x 100 y 88||`` in the **Sprites** drawer. Drag it into ``||loops:on start||``.


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
    
RightButton.setPosition(100, 88)
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
RightButton.setPosition(100, 88)
```

## Step 3 - Setup a label
Now that we have an Right button, we will also want to create an 'Auto Baker' label for it.
Find ``||sprites:set AutoBakerLabel to sprite of kind Player||`` in the **Sprites** drawer. Drag it into ``||loops:on start||``.
Find ``||sprites:set AutoBakerLabel position to x 100 y 99||`` in the **Sprites** drawer. Drag it into ``||loops:on start||``.

```blockconfig.local
let AutoBakerLabel = sprites.create(img`
    ..ffffffffffffffffffffffffffffffffffffffffffffff..
    .f1111111111111111111111111111111111111111111111f.
    f111ff11f11f1fff1ffff1111fff111ff11f11f1fff1fff11f
    f11f11f1f11f11f11f11f1111f1f11f11f1f1f11f111f1f11f
    f11ffff1f11f11f11f11f1ff1ffff1ffff1ff111ff11fff11f
    f11f11f1f11f11f11f11f1111f11f1f11f1f1f11f111ff111f
    f11f11f1ffff11f11ffff1111ffff1f11f1f11f1fff1f1f11f
    .f1111111111111111111111111111111111111111111111f.
    ..ffffffffffffffffffffffffffffffffffffffffffffff..
    `, SpriteKind.Player)
AutoBakerLabel.setPosition(100, 99)
```

```blocks
let AutoBakerLabel = sprites.create(img`
    ..ffffffffffffffffffffffffffffffffffffffffffffff..
    .f1111111111111111111111111111111111111111111111f.
    f111ff11f11f1fff1ffff1111fff111ff11f11f1fff1fff11f
    f11f11f1f11f11f11f11f1111f1f11f11f1f1f11f111f1f11f
    f11ffff1f11f11f11f11f1ff1ffff1ffff1ff111ff11fff11f
    f11f11f1f11f11f11f11f1111f11f1f11f1f1f11f111ff111f
    f11f11f1ffff11f11ffff1111ffff1f11f1f11f1fff1f1f11f
    .f1111111111111111111111111111111111111111111111f.
    ..ffffffffffffffffffffffffffffffffffffffffffffff..
    `, SpriteKind.Player)
AutoBakerLabel.setPosition(100, 99)
```



## Step 4 — Add a buy auto baker button

We need a way to buy an auto baker. Let's use the **Right** button on the controller (the Right arrow key on a keyboard).

Add a new ``||controller:on right button pressed||`` event.

Inside it, add an ``||logic:if/else||`` block that checks: **if cookies >= autoBakerCost**.

```blockconfig.local
controller.right.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
    } else {
    }
})
```

```blocks
controller.right.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
    } else {
    }
})
```

## Step 5 — Buy the auto baker

Inside the **if** branch (when the player can afford it):
1. Subtract ``autoBakerCost`` from ``cookies``
2. Add **1** to ``autoBakers``
3. Update the score
4. Make the cost go up a little (multiply by 1.5 and round — find ``||math:round||`` in the Math drawer)

```blocks
controller.right.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
        cookies -= autoBakerCost
        autoBakers += 1
        info.setScore(cookies)
        autoBakerCost = Math.round(autoBakerCost * 1.5)
    } else {
        game.showLongText("Need " + autoBakerCost + " cookies for an auto baker!", DialogLayout.Bottom)
    }
})
```

## Step 6 — The loop! (ITERATION)

Here comes the important part — the **loop**!

Find ``||game:on game update every 500 ms||`` in the **Game** drawer. Drag it out as a new block. Change the time to **1000** milliseconds (1 second).

This block runs its code **every 1 second**, automatically, forever. That is **iteration** — your code repeats!

```blockconfig.local
game.onUpdateInterval(1000, function () {
})
```

```blocks
game.onUpdateInterval(1000, function () {
})
```

## Step 7 — Bake inside the loop

Inside the ``||game:on game update every 1000 ms||`` block, add an ``||logic:if||`` block:

**if autoBakers > 0** — then add ``autoBakers`` to ``cookies`` and update the score.

We use **if** here (branching inside iteration!) because we only want to add cookies if there are actually some auto bakers working.

```blockconfig.local
if (autoBakers > 0) {
    cookies += autoBakers
    info.setScore(cookies)
}
```

```blocks
game.onUpdateInterval(1000, function () {
    if (autoBakers > 0) {
        cookies += autoBakers
        info.setScore(cookies)
    }
})
```

## Step 8 — Test your auto baker!

Press **Play** and:

1. Bake **50 cookies** by pressing A many times
2. Press the **right arrow** to buy an auto baker
3. Watch the score — it should go up by 1 every second automatically, without pressing anything!
4. Try buying 2 or 3 auto bakers — they all run at once in the loop!

**Think about it:** What happens inside the loop if ``autoBakers`` is 0? (Nothing — the if condition is false!)

## You used iteration! @showdialog

Incredible! Your bakery runs itself!

**What you built:**
- An ``on game update every 1000 ms`` block — a loop that repeats every second
- Branching inside the loop to only bake when auto bakers exist
- An upgrade purchase with another if/else check

**What this means in the Australian Curriculum (AC9TDI4P02):** You implemented an algorithm with *iteration* — your code repeats automatically. You also combined it with *branching* — the loop only does something when the condition is true.

**Next up:** Activity 5 — you will add a **win condition** and put everything together to complete your Cookie Clicker game!
