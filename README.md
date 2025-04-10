<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Movie Recommendation System</title>
    <link rel="stylesheet" href="style.css">
</head>

<body>
    <header>
        <h1>Movie Recommendation System</h1>
    </header>

    <section>
        <h2>Problem</h2>
        <p>
            Streaming platforms like <strong>Netflix</strong> and <strong>Disney+</strong> rely heavily on recommendation systems to enhance user engagement and provide personalized content. Without such systems, users might struggle to find content they enjoy, leading to frustration and decreased platform usage. The problem is, how do we recommend the right movies to a user who might have varied preferences and tastes?
        </p>

        <h2>Solution</h2>
        <p>
            I built a <strong>Movie Recommendation System</strong> that suggests movies based on a given movie title. The system uses <strong>content-based filtering</strong>, where movie recommendations are based on similarities in <strong>descriptions</strong> and <strong>genres</strong>. Using the <strong>TF-IDF Vectorization</strong> technique and <strong>Cosine Similarity</strong>, it analyzes and compares movie descriptions to suggest similar movies.
        </p>
        <p>
            The goal is to help users discover new movies they might enjoy based on the content they've already watched.
        </p>
    </section>

    <section>
        <h2>Technologies Used</h2>
        <ul>
            <li><strong>Python</strong></li>
            <li><strong>TMDb API</strong> (Movie data)</li>
            <li><strong>TF-IDF Vectorization</strong> (Text representation)</li>
            <li><strong>Cosine Similarity</strong> (Similarity calculation)</li>
            <li><strong>Gradio</strong> (Web interface)</li>
        </ul>
    </section>

    <section>
        <h2>Features</h2>
        <ul>
            <li>Fetches movie data from the <strong>TMDb API</strong>.</li>
            <li>Uses <strong>TF-IDF Vectorization</strong> and <strong>Cosine Similarity</strong> to calculate movie similarities.</li>
            <li>User-friendly <strong>Gradio</strong> interface for instant recommendations.</li>
        </ul>
    </section>

    <section>
        <h2>How It Works</h2>
        <h3>1. Data Collection</h3>
        <p>
            I fetched data for over 1,000 popular movies using the <strong>TMDb API</strong>. This includes data such as:
        </p>
        <ul>
            <li>Title</li>
            <li>Genres</li>
            <li>Overview (Movie Description)</li>
            <li>Popularity & Ratings</li>
        </ul>

        <h3>2. Data Cleaning</h3>
        <p>
            I preprocessed the movie data, handling missing values, formatting genres, and combining text columns (overview + genres) for better analysis.
        </p>

        <h3>3. Recommendation Algorithm</h3>
        <p>
            <strong>TF-IDF Vectorization</strong>: Converts movie descriptions and genres into numerical vectors.
        </p>
        <p>
            <strong>Cosine Similarity</strong>: Compares these vectors and finds movies with the most similar content.
        </p>

        <h3>4. Web App</h3>
        <p>
            I built a <strong>Gradio</strong> web interface, allowing users to enter a movie title and get <strong>5 similar movie recommendations</strong> instantly.
        </p>
    </section>

    <section>
        <h2>Screenshot</h2>
        <img src="images/screenshot.png" alt="Movie Recommendation System Screenshot" width="600" />
    </section>

    <section>
        <h2>Installation Instructions</h2>
        <p>To run this project locally:</p>
        <ol>
            <li>Clone the repository:
                <pre><code>git clone https://github.com/yourusername/movie-recommendation.git</code></pre>
            </li>
            <li>Install the dependencies:
                <pre><code>pip install -r requirements.txt</code></pre>
            </li>
            <li>Run the app:
                <pre><code>python app.py</code></pre>
            </li>
            <li>The web app will open in your browser. Enter a movie title, and get recommendations!</li>
        </ol>
    </section>

    <section>
        <h2>Example</h2>
        <p>Search for: <strong>Maze Runner</strong></p>
        <p>The system will return recommendations like:</p>
        <ul>
            <li>Maze Runner: The Death Cure</li>
            <li>Maze Runner: The Scorch Trials</li>
            <li>Tomorrow Before After</li>
            <li>Maze Runner: The Maze Trials</li>
        </ul>
    </section>

    <section>
        <h2>Contributing</h2>
        <p>
            Feel free to fork the repository and submit pull requests for any improvements or fixes!
        </p>
    </section>

    <section>
        <h2>License</h2>
        <p>
            This project is licensed under the MIT License - see the <a href="LICENSE">LICENSE</a> file for details.
        </p>
    </section>

    <section>
        <h2>Contact</h2>
        <p>
            Your Name - <a href="https://twitter.com/yourhandle" target="_blank">@YourTwitterHandle</a>
        </p>
    </section>
</body>

</html>
