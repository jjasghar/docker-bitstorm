# docker-bitstorm

## Scope

This creates a bittorrent tracker based on [bitstorm](https://github.com/petcap/bitstorm) on
Kubernetes. And suprisingly it's a great way to demo how to get a PHP app running on Kubernetes too!

**NOTE**: USE AT YOUR OWN RISK, I TAKE NO RESPONSIBILITY ON WHAT YOU SHARE.

## Usage

You can run this via the Kubernetes manifest in the [k8s](./k8s) directory.

```bash
vi ./k8s/deployment.yaml # you should change the external-dns lines
kubectl apply -f ./k8s/deployment.yaml
```

## Announcing a torrent

If you would like to announce your torrent, you'll need your DNS entry, with something
along the lines of this:

```
http://tracker.DOMAIN.TLD/announce.php
```

## Stats on the tracker

> Check how do it via the `announce.php` file.

## License & Authors

If you would like to see the detailed LICENSE click [here](./LICENSE).

- Author: JJ Asghar <awesome@ibm.com>

```text
Copyright:: 2021- IBM, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
