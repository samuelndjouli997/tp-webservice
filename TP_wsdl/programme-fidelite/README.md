# Il s'agit d'un document Web Services Description Language (WSDL) pour un service de programme de fidélité. Le service fournit une fonctionnalité pour récupérer le solde de points d'un client en fonction de son ID.

# Espace de noms cible
L'espace de noms cible de ce service est http://example.com/fidelityprogram.

# Types
Les types définis pour ce service comprennent :

CustomerID : Un élément de chaîne de caractères représentant l'ID d'un client.
PointsBalance : Un élément entier représentant le solde de points de fidélité pour un client.
GetPointsRequest : Un élément de type complexe représentant une demande pour récupérer les points pour un client.
GetPointsResponse : Un élément de type complexe représentant la réponse du service lors de la récupération du solde de points pour un client.
Messages
Ce service définit deux messages :

GetPointsRequest : Un message utilisé pour demander le solde de points pour un client.
GetPointsResponse : Un message utilisé pour répondre avec le solde de points pour un client.
Type de port
Le type de port FidelityProgramPortType définit une seule opération :

GetPoints : Une opération utilisée pour récupérer le solde de points pour un client. L'opération prend un message GetPointsRequest en entrée et renvoie un message GetPointsResponse en sortie.
# Liaison
La liaison FidelityProgramBinding spécifie le protocole de transport et le format de message pour le type de port FidelityProgramPortType. Ce service utilise SOAP sur HTTP et le format de message de style document.

# Service
Le service FidelityProgramService définit un seul port :

FidelityProgramPort : Un port qui utilise la liaison FidelityProgramBinding et est situé à l'adresse http://example.com/fidelityprogram. Ce port fournit l'accès à l'opération GetPoints du type de port FidelityProgramPortType.