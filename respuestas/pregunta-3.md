MATCH (p:Persona) OPTIONAL MATCH (p)-[:AMIGO_DE]->(a:Persona) WITH p, count(a) AS num_amigos OPTIONAL MATCH (p)-[:PARTICIPA_EN]->(pr:Proyecto) RETURN p.nombre, num_amigos, count(pr) AS num_proyectos
