# Service de Paiements
Ce service de paiements permet de traiter des transactions de paiement en utilisant le protocole SOAP. L'opération MakePayment permet de réaliser une transaction en prenant en entrée un PaymentRequest qui contient les informations de paiement, et renvoie un PaymentResponse qui contient l'identifiant de transaction et le statut de la transaction.

## Fonctionnalités
Traitement de transactions de paiement en ligne
Prise en charge de différentes devises et cartes de crédit
Sécurité accrue en utilisant le protocole SOAP

## Utilisation
Pour utiliser ce service, vous pouvez générer un client SOAP à partir du fichier WSDL fourni. Ensuite, vous pouvez appeler l'opération MakePayment en fournissant un objet PaymentRequest contenant les informations de paiement. Le service renverra un objet PaymentResponse contenant l'identifiant de transaction et le statut de la transaction.