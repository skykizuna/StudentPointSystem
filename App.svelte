<script>
    let students = [
        { name: "Matthew ", points: 0 },
        { name: "Lim Sheng Wei", points: 0 },
        { name: "Keith ", points: 0 },
			  { name: "Tan Yan Ryu", points: 0 },
			  { name: "Quincy ", points: 0 },
    ];

    function changePoints(index, amount) {
        students[index].points += amount;
    }

	 let src = 'https://media1.giphy.com/media/4XZAPHsKaY21W/giphy.gif?cid=6c09b9520lgw0sp8zkkcilfes84yhznva6nordi9ebvpctcm&ep=v1_gifs_search&rid=giphy.gif&ct=g';
</script>

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
<h1>Program E: Sun 5pm</h1>
<h4>Teacher: Yasmin Amani</h4>
<img {src} alt="dance">
<table class="table table-bordered table-striped mt-3">
    <thead>
        <tr>
            <th>Name</th>
            <th>Points</th>
        </tr>
    </thead>
    <tbody>
        {#each students as student, index}
        <tr>
            <td>{student.name}</td>
            <td>{student.points}<br> 
							<button class="btn btn-danger btn-sm" on:click={() => changePoints(index, -1)}>&lt;</button>
              <button class="btn btn-success btn-sm" on:click={() => changePoints(index, 1)}>&gt;</button></td>
        </tr>
        {/each}
    </tbody>
</table>

<h5>How to earn points:</h5>
<ul>
	<li>1 point - for every basic assignment done</li>
	<li>1 point - if code with AI for the chapter is explored</li>
	<li>2 points - if finished until advanced level</li>
	<li>5 points - for doing own project</li>
</ul>

<h5>Things students can earn with points:</h5>
<ol>
	<li>"Silly Rule for a Day" (25 points) – They get to add a fun class rule like "Speak in emojis for 5 minutes."</li>
	<li>Class Playlist Contribution (10 points) – They can suggest a song for a class coding session playlist.</li>
	<li>"Ask the Teacher Anything" Pass (30 points) – A one-on-one session where they can ask coding questions (or fun ones!).</li>
</ol>

<h6>Badge Point System</h6>
<uL>
	<li>10 points - 🏅 Code Explorer Badge</li>
	<li>20 points - 🚀 Svelte Sprinter Badge</li>
	<li>30 points - 🧠 Logic Master Badge</li>
	<li>50 points - 🌟 Creative Coder Badge</li>
</uL>
