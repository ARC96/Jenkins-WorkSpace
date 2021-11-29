node {
  def remote = [:]
  remote.name = 'Rakuten-mon'
  remote.host = '172.24.72.196'
  remote.user = 'ubuntu'
  remote.password = 'root'
  remote.allowAnyHosts = true
  stage('Remote SSH') {
    writeFile file: 'abc.sh', text: 'ls -lrt'
    sshScript remote: remote, script: "abc.sh"
  }
}
