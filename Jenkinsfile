@Library('starry-ci@latest') _

inFirmwareDevContainer('crown') {
    simpleCheckout(withSubmodules: false)

    // We don't need to run a real CI job in here since we haven't changed
    // any source, just build options.
    stage ('Dummy job') {
        sh 'cargo fmt'
    }
}
