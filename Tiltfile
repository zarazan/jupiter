load('ext://helm_resource', 'helm_resource', 'helm_repo')

helm_repo('cockroachdb-repo', 'https://charts.cockroachdb.com/')
helm_resource('cockroachdb', 'cockroachdb-repo/cockroachdb', flags=[
    "--version", "7.0.0",
    "--set", "tls.enabled=false",
    "--set", "config.single-node=true",
    "--set", "statefulset.replicas=1",
