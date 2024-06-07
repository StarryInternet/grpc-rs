@Library('starry-ci@05ef34767e7910d624a7378aeaeb0a34f5055443') _

inFirmwareDevContainer('crown', imageTag: "development-20240606T142800") {
    simpleCheckout(withSubmodules: false)

    // We don't need to run a real CI job in here since we haven't changed
    // any source, just build options.
    stage ('Dummy job') {
        sh 'cargo fmt'
    }
}
