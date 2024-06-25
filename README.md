# InfraHub repo

poetry run infrahubctl run .generators/generate_topology.py topology=EQX-CHI
poetry run infrahubctl run .generators/generate_network-services.py topology=EQX-CHI type=layer2
poetry run infrahubctl run .generators/generate_network-services.py topology=EQX-CHI type=layer3 vrf=production
poetry run infrahubctl render device_arista device=EQX-CHI-leaf1


