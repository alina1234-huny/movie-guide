<?php
session_start();

// Проверяем, есть ли данные в сессии
if (!isset($_SESSION['user_data'])) {
    header('Location: index.html');
    exit();
}

$userData = $_SESSION['user_data'];
$userName = $userData['userName'];
$genreData = $userData['genre_data'];
$careerGuide = $userData['careerGuide'];
$professionalRecommendations = $userData['professional_recommendations'];

// Очищаем сессию после использования
unset($_SESSION['user_data']);
?>
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ваши рекомендации - КиноГид</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <!-- Анимированные волны -->
    <div class="waves">
        <div class="wave wave-1"></div>
        <div class="wave wave-2"></div>
        <div class="wave wave-3"></div>
    </div>

    <div class="results-container">
        <div class="results-content fade-in">
            <!-- Заголовок -->
            <div class="results-header">
                <h1>👋 Привет, <?php echo $userName; ?>!</h1>
                <p>Мы подобрали для вас лучшие фильмы в жанре <?php echo $genreData['name']; ?></p>
            </div>
            
            <!-- Описание жанра -->
            <div class="genre-description">
                <h2>Жанр: <?php echo $genreData['name']; ?></h2>
                <p><?php echo $genreData['description']; ?></p>
            </div>

            <!-- Рекомендованные фильмы -->
            <div class="movies-section">
                <h3>🎬 Рекомендованные фильмы:</h3>
                <div class="movies-grid">
                    <?php foreach ($genreData['movies'] as $movie): ?>
                    <div class="movie-card">
                        <div class="movie-image">
                            <img src="<?php echo $movie['image']; ?>" alt="<?php echo $movie['title']; ?>" 
                                 onerror="this.src='data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzAwIiBoZWlnaHQ9IjIwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48cmVjdCB3aWR0aD0iMTAwJSIgaGVpZ2h0PSIxMDAlIiBmaWxsPSIjZjBmMGYwIi8+PHRleHQgeD0iNTAlIiB5PSI1MCUiIGZvbnQtZmFtaWx5PSJBcmlhbCIgZm9udC1zaXplPSIxNiIgZmlsbD0iIzk5OSIgdGV4dC1hbmNob3I9Im1pZGRsZSIgZHk9Ii4zZW0iPk5vIEltYWdlPC90ZXh0Pjwvc3ZnPg=='">
                        </div>
                        <div class="movie-info">
                            <h4><?php echo $movie['title']; ?></h4>
                            <a href="<?php echo $movie['link']; ?>" target="_blank" class="watch-link">
                                📺 Смотреть на VK Video
                            </a>
                        </div>
                    </div>
                    <?php endforeach; ?>
                </div>
            </div>

            <!-- Профессиональные рекомендации (ПОКАЗЫВАЕМ ВСЕГДА) -->
            <div class="career-recommendations">
                <h3>🎓 Вам будет интересно узнать</h3>
                <p>Эти фильмы помогут вам узнать больше о разных профессиях:</p>
                
                <div class="profession-cards">
                    <?php 
                    // Собираем все профессии из рекомендованных фильмов
                    $allProfessions = [];
                    foreach ($genreData['movies'] as $movie) {
                        if (isset($movie['professions'])) {
                            $allProfessions = array_merge($allProfessions, $movie['professions']);
                        }
                    }
                    $allProfessions = array_unique($allProfessions);
                    
                    // Показываем рекомендации для каждой профессии
                    foreach ($allProfessions as $profession) {
                        if (isset($professionalRecommendations[$profession])) {
                            $profData = $professionalRecommendations[$profession];
                    ?>
                    <div class="profession-card">
                        <h4>👤 Профессия: <?php echo ucfirst($profession); ?></h4>
                        <p class="prof-description"><?php echo $profData['description']; ?></p>
                        <div class="recommended-films">
                            <strong>Рекомендуемые фильмы:</strong>
                            <ul>
                                <?php foreach ($profData['films'] as $film): ?>
                                <li>🎬 <?php echo $film; ?></li>
                                <?php endforeach; ?>
                            </ul>
                        </div>
                    </div>
                    <?php 
                        }
                    } 
                    ?>
                </div>
            </div>

            <!-- Навигация -->
            <div class="navigation">
                <a href="index.html" class="back-button">⟵ Назад к форме</a>
            </div>
        </div>
    </div>
</body>
</html>
