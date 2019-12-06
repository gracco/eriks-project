job('python-ip-script') {
    scm {
        git {
            remote {
                name('python-ip-script')
                url('https://github.com/beerkeeper/python-ip-script')
            }
        }
    }
    steps {
        shell('pip install -r requirements.txt && python main.py')
    }
}