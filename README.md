# InfraHub repo

poetry run infrahubctl run .generators/generate_topology.py topology=eqx-chi
poetry run infrahubctl run .generators/generate_network-services.py topology=eqx-chi type=layer2
poetry run infrahubctl run .generators/generate_network-services.py topology=eqx-chi type=layer3 vrf=production
poetry run infrahubctl render device_arista device=eqx-chi-leaf1


