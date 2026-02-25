const movies = [
    {
        title: "Inception",
        genre: "Sci-Fi",
        poster: "https://image.tmdb.org/t/p/w500/qmDpIHrmpJINaRKAfWQfftjCdyi.jpg"
    },
    {
        title: "Interstellar",
        genre: "Sci-Fi",
        poster: "https://image.tmdb.org/t/p/w500/gEU2QniE6E77NI6lCU6MxlNBvIx.jpg"
    },
    {
        title: "Titanic",
        genre: "Love",
        poster: "https://image.tmdb.org/t/p/w500/9xjZS2rlVxm8SFx8kPC3aIGCOYQ.jpg"
    },
    {
        title: "La La Land",
        genre: "Love",
        poster: "https://image.tmdb.org/t/p/w500/uDO8zWDhfWwoFdKS4fzkUJt0Rf0.jpg"
    },
    {
        title: "Shutter Island",
        genre: "Psycho Thriller",
        poster: "https://image.tmdb.org/t/p/w500/4GDy0PHYX3VRzUtwK5ysFbg9HEx.jpg"
    },
    {
        title: "Gone Girl",
        genre: "Psycho Thriller",
        poster: "https://image.tmdb.org/t/p/w500/qymaJhucquUwjpb8oiqynMeXnID.jpg"
    },
    {
        title: "Gladiator",
        genre: "Action",
        poster: "https://image.tmdb.org/t/p/w500/ty8TGRuvJLPUmAR1H1nRIsgwvim.jpg"
    },
    {
        title: "The Shawshank Redemption",
        genre: "Drama",
        poster: "https://image.tmdb.org/t/p/w500/q6y0Go1tsGEsmtFryDOJo3dEmqu.jpg"
    }
];

const genreColors = {
    "All": "#f7d6d0",              // creamish red
    "Action": "#fee2e2",           // soft red
    "Drama": "#ede9fe",            // lavender
    "Sci-Fi": "#e0f2fe",           // blue
    "Love": "#ffe4e6",             // pink
    "Psycho Thriller": "#e5e7eb"   // grey
};

const container = document.getElementById("movieContainer");

function displayMovies(list) {
    container.innerHTML = "";
    list.forEach(movie => {
        container.innerHTML += `
            <div class="movie-card">
                <img src="${movie.poster}" alt="${movie.title}">
                <div class="movie-info">
                    <h3>${movie.title}</h3>
                    <span class="tag">${movie.genre}</span>
                </div>
            </div>
        `;
    });
}

function filterMovies(genre) {
    document.body.style.background = genreColors[genre];

    if (genre === "All") {
        displayMovies(movies);
    } else {
        const filtered = movies.filter(movie => movie.genre === genre);
        displayMovies(filtered);
    }
}

displayMovies(movies);
