MATCH (p:Persona) OPTIONAL MATCH (p)-[:AMIGO_DE]->(a:Persona) OPTIONAL MATCH (p)-[:PARTICIPA_EN]->(pr:Proyecto) RETURN p.nombre, count(DISTINCT a) AS num_amigos, count(DISTINCT pr) AS num_proyectos
