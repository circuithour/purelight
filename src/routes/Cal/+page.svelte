<script>
    import { onMount } from "svelte";
    import Header from "../../lib/Header.svelte";

    let daysInMonth = 31;
    let today = new Date().getDate();
    let currentMonth = new Date().getMonth(); // Get the current month
    let monthNames = [
        "January",
        "February",
        "March",
        "April",
        "May",
        "June",
        "July",
        "August",
        "September",
        "October",
        "November",
        "December",
    ];
    let monthName = monthNames[currentMonth];
    let firstDayOfWeek = new Date(
        new Date().getFullYear(),
        currentMonth,
        1
    ).getDay();
    const weekdays = ["Sun", "Mon", "Tue", "Wed", "Thu", "Fri", "Sat"];

    function formatDate(date) {
        return date < 10 ? `0${date}` : `${date}`;
    }

    // Calculate the number of empty placeholders
    let emptyPlaceholders = Array.from({ length: firstDayOfWeek }, () => "");

    let calendarDates = Array.from(
        { length: daysInMonth },
        (_, index) => index + 1
    );

    onMount(() => {
        console.log(currentMonth);
    });
</script>

<main>
    <Header />

    <div id="maincontainer" class="container">
        <div class="container" id="list" />
        <div class="container" id="dates">
            <span id="month">{monthName}</span>
            <div class="date-grid">
                {#each weekdays as weekday}
                    <div class="weekday-header">{weekday}</div>
                {/each}
                {#each emptyPlaceholders as _}
                    <div class="date-box empty" />
                {/each}
                {#each calendarDates as date}
                    <div class={date === today ? "date-box today" : "date-box"}>
                        <div class="date-number">{formatDate(date)}</div>
                    </div>
                {/each}
            </div>
        </div>
        <div class="container" id="unsure" />
    </div>
</main>

<style>
    main {
        overflow: hidden;
    }
    .weekday-header {
        font-weight: bold;
        text-align: center;
        padding: 5px;
    }

    .date-box {
        background-color: #4a4a5315;
        border: 1px solid transparent;
        border-radius: 15px;
        width: auto;
        padding: 10px;
        box-sizing: border-box;
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .date-number {
        font-size: 20px;
        margin-bottom: 5px;
    }

    .empty {
        visibility: hidden;
    }

    .note {
        width: 100%;
        height: 100px; /* Adjust this according to your design */
        border: none;
        resize: none;
        padding: 5px;
        box-sizing: border-box;
        background-color: transparent;
    }

    .today {
        color: red;
    }
    #maincontainer {
        padding: 1.5rem;
        display: flex;
        height: 100vh;
        gap: 10px;
    }

    .container {
        flex: 1;
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: 24px;
        color: white;
        height: 90%;
        border: solid 1px rgba(0, 0, 0, 0.144);
        background-color: #03031f25;
        border-radius: 15px;
    }

    #list {
        flex: 0 0 15%;
    }

    #dates {
        flex-direction: column;
        flex: 0 0 70%;
    }

    .date-box {
        background-color: #4a4a5315;
        border: 1px solid transparent;
        border-radius: 15px;
        width: auto; /* Adjust this according to your design */
        height: 180%; /* Adjust this according to your design */
        padding: 10px;
        box-sizing: border-box;
    }
    .date-grid {
        display: grid;
        grid-template-columns: repeat(7, 1fr);
        gap: 50px;
        width: 1000px;
    }

    #unsure {
        flex: 0 0 15%;
    }
</style>
