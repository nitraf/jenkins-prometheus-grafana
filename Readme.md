# Jenkins. Prometheus.Grafana
## Forked from [gangsta/jenkins-prometheus-grafana](https://github.com/gangsta/jenkins-prometheus-grafana)

To get started, perform a git clone on this repository. Make sure you have [Vagrant installed](https://docs.vagrantup.com/v2/installation/), [VirtualBox](https://www.virtualbox.org/wiki/Downloads) or [LibVirt](https://libvirt.org/).

The repository will install for you Jenkins 2.249.1, Prometheus v2.23.0 , Grafana 7.3.5 .

## Final view
![Jenkins: Performance and Health Overview](https://grafana.com/api/dashboards/9964/images/6247/image)

Start with Git Clone
```
git clone https://github.com/gangsta/jenkins-prometheus-grafana
cd jenkins-prometheus-grafana
vagrant up - provider virtualbox
or
vagrant up - provider libvirt
```

Once vagrant is done provisioning the VMs run `vagrant status` to confirm all instances are running:

## Visit the web UI by browsing to:

```bash
Jenkins    http://192.168.33.10:8080/
Prometheus http://192.168.33.10:9090/
Grafana    http://192.168.33.10:3000/

"For Login Use: admin:admin"
```

## Grafana Dashboard:
Dashboards will be automatically provisioned to Grafana:
- Jenkins: Performance and Health Overview
- Prometheus 2.0 Stats


## If you want to login into Vagrant VM run:
```bash
vagrant ssh
```

## When you're done, you can shut down the cluster using:

```bash
vagrant destroy -f
```
