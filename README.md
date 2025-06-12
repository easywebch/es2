<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EasyWeb - Sites Web Clé en Main à partir de 600 CHF</title>
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.2.19/dist/tailwind.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&family=Open+Sans:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@fortawesome/fontawesome-free@6.4.0/css/all.min.css">
    <style>
        :root {
            --blue-tech: #2563EB;
            --orange-energy: #F97316;
            --gray-sophisticated: #374151;
        }
        
        .font-montserrat { font-family: 'Montserrat', sans-serif; }
        .font-opensans { font-family: 'Open Sans', sans-serif; }
        
        .bg-gradient-primary {
            background: linear-gradient(135deg, var(--blue-tech) 0%, var(--orange-energy) 100%);
        }
        
        .text-blue-tech { color: var(--blue-tech); }
        .text-orange-energy { color: var(--orange-energy); }
        .bg-blue-tech { background-color: var(--blue-tech); }
        .bg-orange-energy { background-color: var(--orange-energy); }
        .border-blue-tech { border-color: var(--blue-tech); }
        .border-orange-energy { border-color: var(--orange-energy); }
        
        .hover-scale { transition: transform 0.3s ease; }
        .hover-scale:hover { transform: scale(1.05); }
        
        .animate-float {
            animation: float 6s ease-in-out infinite;
        }
        
        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-20px); }
        }
        
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.8s ease;
        }
        
        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
        
        .card-hover {
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(37, 99, 235, 0.1);
        }
        
        .card-hover:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(37, 99, 235, 0.2);
        }
        
        .pulse-orange {
            animation: pulse-orange 2s infinite;
        }
        
        @keyframes pulse-orange {
            0%, 100% { box-shadow: 0 0 0 0 rgba(249, 115, 22, 0.7); }
            70% { box-shadow: 0 0 0 10px rgba(249, 115, 22, 0); }
        }
    </style>
</head>
<body class="font-opensans bg-white">

<!-- Header -->
<header class="bg-white shadow-lg fixed w-full top-0 z-50">
    <nav class="container mx-auto px-6 py-4">
        <div class="flex justify-between items-center">
            <div class="flex items-center">
                <div class="text-3xl font-montserrat font-bold text-blue-tech">
                    <span class="text-orange-energy">Easy</span>Web
                </div>
            </div>
            <div class="hidden md:flex space-x-8">
                <a href="#accueil" class="text-gray-700 hover:text-blue-tech transition duration-300">Accueil</a>
                <a href="#services" class="text-gray-700 hover:text-blue-tech transition duration-300">Services</a>
                <a href="#tarifs" class="text-gray-700 hover:text-blue-tech transition duration-300">Tarifs</a>
                <a href="#contact" class="text-gray-700 hover:text-blue-tech transition duration-300">Contact</a>
            </div>
            <button onclick="scrollToContact()" class="bg-orange-energy text-white px-6 py-2 rounded-full hover:bg-opacity-90 transition duration-300 pulse-orange">
                Être Rappelé
            </button>
        </div>
    </nav>
</header>

<!-- Hero Section -->
<section id="accueil" class="pt-24 pb-16 bg-gradient-primary text-white">
    <div class="container mx-auto px-6">
        <div class="flex flex-col lg:flex-row items-center">
            <div class="lg:w-1/2 lg:pr-10 mb-10 lg:mb-0">
                <h1 class="text-5xl lg:text-6xl font-montserrat font-bold mb-6 animate-float">
                    Sites Web Clé en Main
                </h1>
                <p class="text-2xl mb-4">À partir de</p>
                <div class="text-6xl font-montserrat font-bold mb-6 text-yellow-300">
                    600 CHF
                </div>
                <p class="text-xl mb-8 leading-relaxed">
                    Créez votre présence en ligne avec un site web professionnel, personnalisé et optimisé. 
                    Solution complète sans tracas technique pour le marché suisse !
                </p>
                <div class="flex flex-col sm:flex-row gap-4">
                    <button onclick="scrollToContact()" class="bg-orange-energy text-white px-8 py-4 rounded-full text-lg font-semibold hover:bg-opacity-90 transition duration-300 hover-scale">
                        <i class="fas fa-rocket mr-2"></i>Démarrer Mon Projet
                    </button>
                    <button onclick="scrollToServices()" class="border-2 border-white text-white px-8 py-4 rounded-full text-lg font-semibold hover:bg-white hover:text-blue-tech transition duration-300">
                        <i class="fas fa-info-circle mr-2"></i>En Savoir Plus
                    </button>
                </div>
            </div>
            <div class="lg:w-1/2">
                <img src="https://www.free-mockup.com/wp-content/uploads/edd/2024/09/Responsive-Scene-Device-Free-Mockups-01.jpg" 
                     alt="Mockup site web responsive" 
                     class="w-full h-auto rounded-lg shadow-2xl animate-float">
            </div>
        </div>
    </div>
</section>

<!-- Avantages Section -->
<section class="py-16 bg-gray-50">
    <div class="container mx-auto px-6">
        <h2 class="text-4xl font-montserrat font-bold text-center text-gray-800 mb-12">
            Pourquoi Choisir <span class="text-blue-tech">EasyWeb</span> en Suisse ?
        </h2>
        <div class="grid md:grid-cols-3 gap-8">
            <div class="card-hover bg-white p-8 rounded-xl text-center fade-in">
                <div class="bg-blue-tech text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-coins text-2xl"></i>
                </div>
                <h3 class="text-2xl font-montserrat font-bold mb-4 text-gray-800">Prix Accessible</h3>
                <p class="text-gray-600 leading-relaxed">
                    Sites web professionnels à partir de 600 CHF seulement. Qualité premium sans exploser votre budget suisse.
                </p>
            </div>
            
            <div class="card-hover bg-white p-8 rounded-xl text-center fade-in">
                <div class="bg-orange-energy text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-clock text-2xl"></i>
                </div>
                <h3 class="text-2xl font-montserrat font-bold mb-4 text-gray-800">Livraison Rapide</h3>
                <p class="text-gray-600 leading-relaxed">
                    Votre site web livré clé en main en quelques jours. Plus besoin d'attendre des mois !
                </p>
            </div>
            
            <div class="card-hover bg-white p-8 rounded-xl text-center fade-in">
                <div class="bg-blue-tech text-white w-16 h-16 rounded-full flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-paint-brush text-2xl"></i>
                </div>
                <h3 class="text-2xl font-montserrat font-bold mb-4 text-gray-800">100% Personnalisé</h3>
                <p class="text-gray-600 leading-relaxed">
                    Design unique qui reflète parfaitement votre marque et vos valeurs d'entreprise suisse.
                </p>
            </div>
        </div>
    </div>
</section>

<!-- Services Section -->
<section id="services" class="py-16 bg-white">
    <div class="container mx-auto px-6">
        <h2 class="text-4xl font-montserrat font-bold text-center text-gray-800 mb-4">
            Nos <span class="text-orange-energy">Services</span>
        </h2>
        <p class="text-xl text-gray-600 text-center mb-12 max-w-3xl mx-auto">
            De la création de votre site jusqu'à son succès en ligne, nous vous accompagnons à chaque étape
        </p>
        
        <div class="grid lg:grid-cols-2 gap-12 items-center mb-16">
            <div>
                <img src="https://images.stockcake.com/public/8/4/9/8496ab55-25c7-4fde-a416-0d7bbc9478d7_large/tech-team-working-stockcake.jpg" 
                     alt="Équipe de développement" 
                     class="w-full rounded-xl shadow-2xl">
            </div>
            <div>
                <h3 class="text-3xl font-montserrat font-bold mb-6 text-gray-800">
                    <span class="text-blue-tech">Site Web</span> Clé en Main
                </h3>
                <div class="space-y-4">
                    <div class="flex items-start">
                        <i class="fas fa-check-circle text-orange-energy text-xl mr-4 mt-1"></i>
                        <p class="text-gray-600">Design responsive adapté à tous les écrans</p>
                    </div>
                    <div class="flex items-start">
                        <i class="fas fa-check-circle text-orange-energy text-xl mr-4 mt-1"></i>
                        <p class="text-gray-600">Optimisation SEO pour être visible sur Google Suisse</p>
                    </div>
                    <div class="flex items-start">
                        <i class="fas fa-check-circle text-orange-energy text-xl mr-4 mt-1"></i>
                        <p class="text-gray-600">Formulaires de contact intégrés</p>
                    </div>
                    <div class="flex items-start">
                        <i class="fas fa-check-circle text-orange-energy text-xl mr-4 mt-1"></i>
                        <p class="text-gray-600">Hébergement et nom de domaine .ch inclus</p>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
            <div class="card-hover bg-gradient-to-br from-blue-50 to-blue-100 p-8 rounded-xl">
                <div class="bg-blue-tech text-white w-12 h-12 rounded-lg flex items-center justify-center mb-6">
                    <i class="fas fa-shopping-cart"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">E-Commerce</h4>
                <p class="text-gray-600 mb-4">
                    Boutique en ligne complète avec gestion des produits, paiements sécurisés TWINT/PostFinance et suivi des commandes.
                </p>
                <a href="#contact" class="text-blue-tech font-semibold hover:text-orange-energy transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
            
            <div class="card-hover bg-gradient-to-br from-orange-50 to-orange-100 p-8 rounded-xl">
                <div class="bg-orange-energy text-white w-12 h-12 rounded-lg flex items-center justify-center mb-6">
                    <i class="fas fa-cogs"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">Automatisations</h4>
                <p class="text-gray-600 mb-4">
                    Emails automatiques, SMS, workflows pour optimiser votre relation client et gagner du temps.
                </p>
                <a href="#contact" class="text-orange-energy font-semibold hover:text-blue-tech transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
            
            <div class="card-hover bg-gradient-to-br from-green-50 to-green-100 p-8 rounded-xl">
                <div class="bg-green-500 text-white w-12 h-12 rounded-lg flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-bullhorn"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">Publicité Digitale</h4>
                <p class="text-gray-600 mb-4">
                    Campagnes Google Ads, Facebook Ads et gestion complète de votre publicité en ligne pour le marché suisse.
                </p>
                <a href="#contact" class="text-green-500 font-semibold hover:text-orange-energy transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
            
            <div class="card-hover bg-gradient-to-br from-purple-50 to-purple-100 p-8 rounded-xl">
                <div class="bg-purple-500 text-white w-12 h-12 rounded-lg flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-chart-line"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">Lead Generation</h4>
                <p class="text-gray-600 mb-4">
                    Systèmes de qualification de prospects automatisés pour transformer vos visiteurs en clients.
                </p>
                <a href="#contact" class="text-purple-500 font-semibold hover:text-orange-energy transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
            
            <div class="card-hover bg-gradient-to-br from-pink-50 to-pink-100 p-8 rounded-xl">
                <div class="bg-pink-500 text-white w-12 h-12 rounded-lg flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-pen-fancy"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">Création de Contenu</h4>
                <p class="text-gray-600 mb-4">
                    Rédaction de contenus optimisés, images, vidéos pour alimenter votre site et réseaux sociaux.
                </p>
                <a href="#contact" class="text-pink-500 font-semibold hover:text-orange-energy transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
            
            <div class="card-hover bg-gradient-to-br from-yellow-50 to-yellow-100 p-8 rounded-xl">
                <div class="bg-yellow-500 text-white w-12 h-12 rounded-lg flex items-center justify-center mx-auto mb-6">
                    <i class="fas fa-headset"></i>
                </div>
                <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">Support & Maintenance</h4>
                <p class="text-gray-600 mb-4">
                    Support technique continu, mises à jour et maintenance pour un site toujours performant.
                </p>
                <a href="#contact" class="text-yellow-600 font-semibold hover:text-orange-energy transition duration-300">
                    En savoir plus <i class="fas fa-arrow-right ml-1"></i>
                </a>
            </div>
        </div>
    </div>
</section>

<!-- Tarifs Section -->
<section id="tarifs" class="py-16 bg-gray-50">
    <div class="container mx-auto px-6">
        <h2 class="text-4xl font-montserrat font-bold text-center text-gray-800 mb-4">
            Une Offre <span class="text-orange-energy">Accessible</span>
        </h2>
        <p class="text-xl text-gray-600 text-center mb-12">
            Créer votre site web professionnel n'a jamais été aussi simple et abordable en Suisse
        </p>
        
        <div class="max-w-4xl mx-auto">
            <div class="bg-white rounded-2xl shadow-2xl overflow-hidden">
                <div class="bg-gradient-primary text-white text-center py-8">
                    <h3 class="text-3xl font-montserrat font-bold mb-2">Site Web Clé en Main</h3>
                    <p class="text-xl opacity-90">Tout ce dont vous avez besoin pour démarrer en Suisse</p>
                </div>
                
                <div class="p-8">
                    <div class="text-center mb-8">
                        <div class="text-6xl font-montserrat font-bold text-blue-tech mb-2">600 CHF</div>
                        <p class="text-gray-500">Tarif de démarrage - Projet personnalisé</p>
                    </div>
                    
                    <div class="grid md:grid-cols-2 gap-8 mb-8">
                        <div>
                            <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">✨ Inclus dans l'offre :</h4>
                            <ul class="space-y-3">
                                <li class="flex items-start">
                                    <i class="fas fa-check text-green-500 mr-3 mt-1"></i>
                                    <span class="text-gray-600">Design 100% personnalisé</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-green-500 mr-3 mt-1"></i>
                                    <span class="text-gray-600">Site responsive (mobile/tablette)</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-green-500 mr-3 mt-1"></i>
                                    <span class="text-gray-600">Optimisation SEO pour Google Suisse</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-green-500 mr-3 mt-1"></i>
                                    <span class="text-gray-600">Formulaires de contact</span>
                                </li>
                                <li class="flex items-start">
                                    <i class="fas fa-check text-green-500 mr-3 mt-1"></i>
                                    <span class="text-gray-600">Hébergement 1 an + domaine .ch inclus</span>
                                </li>
                            </ul>
                        </div>
                        
                        <div>
                            <h4 class="text-xl font-montserrat font-bold mb-4 text-gray-800">🚀 Processus simple :</h4>
                            <div class="space-y-4">
                                <div class="flex items-start">
                                    <div class="bg-blue-tech text-white w-8 h-8 rounded-full flex items-center justify-center mr-3 mt-0.5 text-sm font-bold">1</div>
                                    <span class="text-gray-600">Vous nous contactez</span>
                                </div>
                                <div class="flex items-start">
                                    <div class="bg-blue-tech text-white w-8 h-8 rounded-full flex items-center justify-center mr-3 mt-0.5 text-sm font-bold">2</div>
                                    <span class="text-gray-600">Nous analysons vos besoins</span>
                                </div>
                                <div class="flex items-start">
                                    <div class="bg-orange-energy text-white w-8 h-8 rounded-full flex items-center justify-center mr-3 mt-0.5 text-sm font-bold">3</div>
                                    <span class="text-gray-600">Création de votre site</span>
                                </div>
                                <div class="flex items-start">
                                    <div class="bg-green-500 text-white w-8 h-8 rounded-full flex items-center justify-center mr-3 mt-0.5 text-sm font-bold">4</div>
                                    <span class="text-gray-600">Livraison clé en main !</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="text-center">
                        <button onclick="scrollToContact()" class="bg-orange-energy text-white px-12 py-4 rounded-full text-xl font-semibold hover:bg-opacity-90 transition duration-300 hover-scale pulse-orange">
                            <i class="fas fa-phone mr-2"></i>Être Rappelé Maintenant
                        </button>
                        <p class="text-sm text-gray-500 mt-4">Devis gratuit et sans engagement</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Contact Section -->
<section id="contact" class="py-16 bg-white">
    <div class="container mx-auto px-6">
        <h2 class="text-4xl font-montserrat font-bold text-center text-gray-800 mb-4">
            Prêt à <span class="text-blue-tech">Démarrer</span> ?
        </h2>
        <p class="text-xl text-gray-600 text-center mb-12">
            Contactez-nous dès maintenant pour obtenir votre devis personnalisé
        </p>
        
        <div class="max-w-4xl mx-auto">
            <div class="grid lg:grid-cols-2 gap-12">
                <!-- Formulaire principal -->
                <div class="bg-gradient-to-br from-blue-50 to-white p-8 rounded-2xl shadow-xl">
                    <h3 class="text-2xl font-montserrat font-bold mb-6 text-gray-800">
                        <i class="fas fa-paper-plane text-blue-tech mr-2"></i>
                        Demander un Devis
                    </h3>
                    <form id="devisForm" class="space-y-6">
                        <div class="grid md:grid-cols-2 gap-4">
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Prénom *</label>
                                <input type="text" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300" placeholder="Votre prénom">
                            </div>
                            <div>
                                <label class="block text-gray-700 font-semibold mb-2">Nom *</label>
                                <input type="text" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300" placeholder="Votre nom">
                            </div>
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Email *</label>
                            <input type="email" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300" placeholder="votre@email.ch">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Entreprise</label>
                            <input type="text" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300" placeholder="Nom de votre entreprise">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Type de projet *</label>
                            <select required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300">
                                <option value="">Sélectionnez votre projet</option>
                                <option value="site-vitrine">Site vitrine (600 CHF)</option>
                                <option value="e-commerce">Site e-commerce</option>
                                <option value="automatisations">Automatisations marketing</option>
                                <option value="publicite">Gestion publicitaire</option>
                                <option value="autre">Autre projet</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Décrivez votre projet</label>
                            <textarea rows="4" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-tech transition duration-300" placeholder="Parlez-nous de vos besoins, objectifs, délais..."></textarea>
                        </div>
                        <button type="submit" class="w-full bg-blue-tech text-white px-6 py-4 rounded-lg text-lg font-semibold hover:bg-opacity-90 transition duration-300 hover-scale">
                            <i class="fas fa-paper-plane mr-2"></i>Envoyer ma Demande
                        </button>
                    </form>
                </div>
                
                <!-- Demande de rappel -->
                <div class="bg-gradient-to-br from-orange-50 to-white p-8 rounded-2xl shadow-xl">
                    <h3 class="text-2xl font-montserrat font-bold mb-6 text-gray-800">
                        <i class="fas fa-phone text-orange-energy mr-2"></i>
                        Être Rappelé
                    </h3>
                    <p class="text-gray-600 mb-6">
                        Vous préférez qu'on vous appelle ? Laissez-nous vos coordonnées et nous vous rappelons sous 24h !
                    </p>
                    <form id="rappelForm" class="space-y-6">
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Nom complet *</label>
                            <input type="text" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-energy transition duration-300" placeholder="Votre nom complet">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Téléphone *</label>
                            <input type="tel" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-energy transition duration-300" placeholder="+41 76 123 45 67">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Email *</label>
                            <input type="email" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-energy transition duration-300" placeholder="votre@email.ch">
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Meilleur moment pour vous appeler</label>
                            <select class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-energy transition duration-300">
                                <option value="">Indifférent</option>
                                <option value="matin">Matin (9h-12h)</option>
                                <option value="apres-midi">Après-midi (14h-17h)</option>
                                <option value="soir">Début de soirée (17h-19h)</option>
                            </select>
                        </div>
                        <div>
                            <label class="block text-gray-700 font-semibold mb-2">Votre projet en quelques mots</label>
                            <textarea rows="3" class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-orange-energy transition duration-300" placeholder="Décrivez brièvement votre projet..."></textarea>
                        </div>
                        <button type="submit" class="w-full bg-orange-energy text-white px-6 py-4 rounded-lg text-lg font-semibold hover:bg-opacity-90 transition duration-300 hover-scale pulse-orange">
                            <i class="fas fa-phone mr-2"></i>Demander un Rappel
                        </button>
                    </form>
                    
                    <div class="mt-8 p-6 bg-white rounded-xl border-l-4 border-orange-energy">
                        <h4 class="font-bold text-gray-800 mb-2">⚡ Réponse Rapide</h4>
                        <p class="text-sm text-gray-600">
                            Nous nous engageons à vous rappeler sous 24h (jours ouvrés). 
                            Appel gratuit et sans engagement !
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</section>

<!-- Footer -->
<footer class="bg-gray-800 text-white py-12">
    <div class="container mx-auto px-6">
        <div class="flex flex-col md:flex-row justify-between items-center">
            <div class="mb-6 md:mb-0">
                <div class="text-3xl font-montserrat font-bold">
                    <span class="text-orange-energy">Easy</span>Web
                </div>
                <p class="text-gray-300 mt-2">Sites web clé en main à partir de 600 CHF</p>
            </div>
            <div class="text-center md:text-right">
                <p class="text-gray-300 mb-2">Prêt à démarrer votre projet ?</p>
                <button onclick="scrollToContact()" class="bg-orange-energy text-white px-6 py-2 rounded-full hover:bg-opacity-90 transition duration-300">
                    Contactez-nous
                </button>
            </div>
        </div>
        <div class="border-t border-gray-700 mt-8 pt-8 text-center text-gray-400">
            <p>&copy; 2024 EasyWeb Suisse. Tous droits réservés. | Sites web professionnels et services digitaux</p>
        </div>
    </div>
</footer>

<script>
// Smooth scrolling
function scrollToContact() {
    document.getElementById('contact').scrollIntoView({
        behavior: 'smooth'
    });
}

function scrollToServices() {
    document.getElementById('services').scrollIntoView({
        behavior: 'smooth'
    });
}

// Fade in animation on scroll
const observerOptions = {
    threshold: 0.1,
    rootMargin: '0px 0px -50px 0px'
};

const observer = new IntersectionObserver((entries) => {
    entries.forEach(entry => {
        if (entry.isIntersecting) {
            entry.target.classList.add('visible');
        }
    });
}, observerOptions);

document.querySelectorAll('.fade-in').forEach(el => {
    observer.observe(el);
});

// Form submissions
document.getElementById('devisForm').addEventListener('submit', function(e) {
    e.preventDefault();
    
    // Animation de succès
    const button = this.querySelector('button[type="submit"]');
    const originalText = button.innerHTML;
    
    button.innerHTML = '<i class="fas fa-spinner fa-spin mr-2"></i>Envoi en cours...';
    button.disabled = true;
    
    setTimeout(() => {
        button.innerHTML = '<i class="fas fa-check mr-2"></i>Message envoyé !';
        button.className = button.className.replace('bg-blue-tech', 'bg-green-500');
        
        setTimeout(() => {
            button.innerHTML = originalText;
            button.disabled = false;
            button.className = button.className.replace('bg-green-500', 'bg-blue-tech');
            this.reset();
        }, 3000);
    }, 2000);
});

document.getElementById('rappelForm').addEventListener('submit', function(e) {
    e.preventDefault();
    
    // Animation de succès
    const button = this.querySelector('button[type="submit"]');
    const originalText = button.innerHTML;
    
    button.innerHTML = '<i class="fas fa-spinner fa-spin mr-2"></i>Envoi en cours...';
    button.disabled = true;
    
    setTimeout(() => {
        button.innerHTML = '<i class="fas fa-check mr-2"></i>Demande envoyée !';
        button.className = button.className.replace('bg-orange-energy', 'bg-green-500');
        
        setTimeout(() => {
            button.innerHTML = originalText;
            button.disabled = false;
            button.className = button.className.replace('bg-green-500', 'bg-orange-energy');
            this.reset();
        }, 3000);
    }, 2000);
});

// Smooth scroll pour les liens de navigation
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
    anchor.addEventListener('click', function (e) {
        e.preventDefault();
        const target = document.querySelector(this.getAttribute('href'));
        if (target) {
            target.scrollIntoView({
                behavior: 'smooth',
                block: 'start'
            });
        }
    });
});

// Header shadow on scroll
window.addEventListener('scroll', () => {
    const header = document.querySelector('header');
    if (window.scrollY > 100) {
        header.classList.add('shadow-xl');
    } else {
        header.classList.remove('shadow-xl');
    }
});
</script>

</body>
</html>
