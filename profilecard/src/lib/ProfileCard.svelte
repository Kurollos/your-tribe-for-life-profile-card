<script>
    const profile = {
        name: 'Kurollos Yaakoub',
        role: 'Frontend Student',
        introduction:
            'Ik ben een 22-jarige Developer. Ik ben geïnteresseerd in front-end design, omdat ik dol ben op creativiteit en met deze opleiding kan ik mijn kennis uitbreiden.',
        dream:
            'Ik wil graag nieuwe dingen leren zodat ik later in een bedrijf kan werken en designs kan maken.',
        passion:
            'Ik lees fantasyboeken, sport graag buiten en game graag.',
        skills: [
            '💻 Frontend Design',
            '🏆 Samenwerking: ★★★',
            '🔍 Oplettend: ★★',
            '😌 Rustig: ★★★★'
        ]
    };
</script>

<article class="rect-card">
    <div class="rect-card-front">
        <h2>Visitekaartje 2026</h2>

        <div class="card-content">
            <img
                src="/assets/IMG_6652 (4).jpg"
                alt="Profielfoto van {profile.name}"
                width="150"
                height="150"
            />

            <div class="text-content">
                <h2>{profile.name}</h2>

                <p>{profile.role}</p>

                <p>{profile.introduction}</p>

                <h3>Skills & Kwaliteiten</h3>

                <ul>
                    {#each profile.skills as skill}
                        <li>{skill}</li>
                    {/each}
                </ul>

                <h3>Mijn droom</h3>

                <p>{profile.dream}</p>

                <h3>Mijn passie</h3>

                <p>{profile.passion}</p>

                <div class="skills">
                    <span>HTML</span>
                    <span>CSS</span>
                    <span>JS</span>
                </div>
            </div>
        </div>
    </div>
</article>
<style>
    .rect-card {
        max-width: 700px;
        margin: 2rem auto;
        padding: 1.5rem;
        background: #0b1f3a;
        color: white;
        border: 1px solid #163a63;
        border-radius: 1rem;
        box-shadow: 0 4px 12px rgb(0 0 0 / 30%);
    }

    .rect-card-front > h2 {
        margin-top: 0;
        text-align: center;
        color: white;
    }

    .card-content {
        display: flex;
        gap: 1.5rem;
        align-items: flex-start;
    }

    .card-content img {
        width: 150px;
        height: 150px;
        object-fit: cover;
        border-radius: 50%;
        flex-shrink: 0;
        border: 3px solid white;
    }

    .text-content {
        flex: 1;
    }

    .text-content h2 {
        margin-top: 0;
        color: white;
    }

    .text-content h3 {
        margin-bottom: 0.5rem;
        color: #8fc7ff;
    }

    .text-content p {
        line-height: 1.6;
        color: #f1f5f9;
    }

    ul {
        padding-left: 1.5rem;
    }

    li {
        margin-bottom: 0.4rem;
        color: #f1f5f9;
    }

    .skills {
        display: flex;
        gap: 0.5rem;
        margin-top: 1rem;
    }

    .skills span {
        padding: 0.4rem 0.7rem;
        background: #163a63;
        color: white;
        border-radius: 0.5rem;
    }

    @media (max-width: 600px) {
        .card-content {
            flex-direction: column;
        }

        .card-content img {
            width: 120px;
            height: 120px;
        }
    }
</style>