MATCH (p:Persona)-[:AMIGO_DE]->(a:Persona) WITH p, count(a) AS num_amigos WHERE num_amigos > 1 RETURN p.nombre, num_amigos
