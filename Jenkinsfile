@Library('starry-ci@05ef34767e7910d624a7378aeaeb0a34f5055443') _

inFirmwareDevContainer('crown', imageTag: "development-20240606T142800") {
    simpleCheckout(withSubmodules: false)

    withEnv('GRPCIO_SYS_USE_PKG_CONFIG=1') {
        buildRustProject('grpcio', skipLinting: true)
    }
}
