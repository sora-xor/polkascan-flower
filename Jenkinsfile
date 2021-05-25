@Library('jenkins-library' ) _

def pipeline = new org.docker.AppPipeline(steps: this,
    dockerImageName: 'sora2/polkascan-flower',
    dockerRegistryCred: 'bot-sora2-rw',
    gitUpdateSubmodule: true,
    secretScannerExclusion: '.*docs\$|.*options.py\$|.*broker.py\$')
pipeline.runPipeline()