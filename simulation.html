<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Manpower Cost Analysis</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap');

        body {
            font-family: 'Inter', sans-serif;
            background-color: #f8fafc; /* Very light gray */
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
            box-sizing: border-box;
        }

        .container {
            background-color: #ffffff;
            border-radius: 12px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.08);
            padding: 30px;
            width: 100%;
            max-width: 960px; /* Slightly wider */
            text-align: center;
            border: 1px solid #e2e8f0;
            display: flex;
            flex-direction: column;
            gap: 25px;
        }

        h1 {
            font-size: 2.5rem; /* text-4xl */
            font-weight: 700; /* font-bold */
            color: #2d3748; /* Darker gray for headings */
            margin-bottom: 20px;
        }

        .scenario-buttons {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 12px;
            margin-bottom: 25px;
        }

        .scenario-btn {
            padding: 10px 22px;
            background-color: #4299e1; /* Professional blue */
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 0.95rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s ease;
            box-shadow: 0 3px 10px rgba(66, 153, 225, 0.3);
        }

        .scenario-btn:hover {
            background-color: #3182ce; /* Darker blue */
            transform: translateY(-1px);
            box-shadow: 0 4px 12px rgba(66, 153, 225, 0.4);
        }

        .scenario-btn.active {
            background-color: #2b6cb0; /* Even darker blue */
            box-shadow: 0 4px 12px rgba(43, 108, 176, 0.5);
            transform: translateY(-0.5px);
        }

        .simulation-area {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 25px;
        }

        .company-box, .contractor-row {
            background-color: #f7fafc; /* Off-white */
            border-radius: 10px;
            padding: 18px;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 12px;
            box-shadow: inset 0 1px 3px rgba(0, 0, 0, 0.03);
            border: 1px solid #edf2f7;
        }

        .company-box {
            background-color: #e0f2f7; /* Very light blue-green */
            padding: 22px;
            font-size: 1.4rem;
            font-weight: 700;
            color: #2b6cb0; /* Main professional blue */
            border: 1px solid #bee3f8;
            position: relative;
            overflow: hidden;
            flex-direction: column;
        }

        .company-box::before {
            content: 'Company Overview';
            position: absolute;
            top: 8px;
            left: 10px;
            font-size: 0.8rem;
            font-weight: 600;
            color: rgba(43, 108, 176, 0.7);
        }

        .contractor-row {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(130px, 1fr)); /* Slightly wider contractor boxes */
            gap: 12px;
            width: 100%;
        }

        .contractor-box {
            background-color: #ebf8ff; /* Lighter blue */
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 1px 6px rgba(0, 0, 0, 0.05);
            border: 1px solid #90cdf4;
            font-size: 0.9rem;
            font-weight: 600;
            color: #3182ce; /* Professional blue */
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 8px;
            position: relative;
            overflow: hidden;
        }

        .contractor-box::before {
            content: 'Contractor';
            position: absolute;
            top: 5px;
            left: 8px;
            font-size: 0.7rem;
            font-weight: 600;
            color: rgba(49, 130, 206, 0.7);
        }

        .worker-group {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 4px;
        }

        .worker-icon {
            width: 16px;
            height: 16px;
            background-color: #63b3ed; /* Mid blue */
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            color: white;
            font-size: 0.65rem;
            font-weight: 700;
        }

        .results-section {
            background-color: #f0f4f8; /* Muted light blue-gray */
            border-radius: 12px;
            padding: 25px;
            margin-top: 20px;
            border: 1px solid #d8e2ed;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.05);
            text-align: left;
        }

        .result-item {
            font-size: 1.1rem;
            font-weight: 600;
            color: #4a5568; /* Muted gray */
            margin-bottom: 10px;
            display: flex;
            justify-content: space-between;
            align-items: baseline;
        }
        .result-item strong {
            color: #2d3748;
        }

        .result-value {
            font-size: 1.6rem; /* Slightly smaller for professional look */
            font-weight: 700;
            color: #48bb78; /* Muted green for positive */
            animation: countUp 1.5s ease-out forwards;
            display: inline-block;
            margin-left: 10px;
        }

        #originalAnnualCompanyCost, #newAnnualCompanyCost {
             color: #e53e3e; /* Muted red for costs */
        }
        #costPercentageIncrease {
            color: #e53e3e; /* Muted red for cost increase percentage */
        }

        .text-green-700 { color: #38a169; } /* Muted green for annual inc */
        .text-gray-700 { color: #4a5568; } /* Muted gray for current annual */


        /* Animation for number counting */
        @keyframes countUp {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Particle animation (simplified for demonstration) */
        .particle {
            position: absolute;
            background-color: rgba(255, 204, 0, 0.7); /* Slightly muted gold */
            border-radius: 50%;
            width: 7px;
            height: 7px;
            opacity: 0;
            transform: translateY(0);
            transition: opacity 0.5s ease-out, transform 1s linear;
        }

        .flow-path {
            position: absolute;
            top: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 2px;
            background-color: rgba(66, 153, 225, 0.2); /* Faint blue line */
            height: 0;
            transition: height 0.5s ease-out;
            z-index: 0;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            h1 {
                font-size: 1.75rem;
            }
            .container {
                padding: 20px;
                gap: 15px;
            }
            .scenario-buttons {
                flex-direction: column;
                gap: 10px;
            }
            .scenario-btn {
                width: 100%;
            }
            .contractor-row {
                grid-template-columns: 1fr;
            }
            .company-box, .contractor-box, .results-section {
                padding: 15px;
            }
            .result-item {
                font-size: 0.95rem;
                flex-direction: column;
                align-items: flex-start;
            }
            .result-value {
                font-size: 1.2rem;
                margin-left: 0;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Manpower Cost Analysis</h1>

        <div class="scenario-buttons">
            <button id="btnReset" class="scenario-btn">Reset to Current</button>
            <button id="btn100" class="scenario-btn">Increase by ₹100/day</button>
            <button id="btn1000" class="scenario-btn">Increase by ₹1000/day</button>
        </div>

        <div class="simulation-area">
            <div class="company-box">
                <p>Total Manpower: <span id="totalManpower"></span></p>
                <div class="flow-path" id="flowPath"></div>
            </div>

            <div class="contractor-row" id="contractorRow">
                <!-- Contractor boxes will be dynamically generated here -->
            </div>
        </div>

        <div class="results-section">
            <div class="result-item">
                <strong>Original Annual Cost to Company:</strong>
                <span class="result-value" id="originalAnnualCompanyCost">₹0</span>
            </div>
            <div class="result-item">
                <strong>New Annual Cost to Company:</strong>
                <span class="result-value" id="newAnnualCompanyCost">₹0</span>
            </div>
            <div class="result-item">
                <strong>Percentage Increase in Annual Cost:</strong>
                <span class="result-value" id="costPercentageIncrease">0.00%</span>
            </div>
        </div>
    </div>

    <script>
        const numContractors = 6;
        const workersPerContractor = 8; // Each contractor still has 8 workers total
        const totalManpower = numContractors * workersPerContractor; // Total manpower remains 48
        const annualEarningsPerContractor = 7200000; // ₹72 lakhs per contractor annually

        // Calculate the base daily rate per manpower based on target annual earnings per contractor
        // (72 lakhs per contractor / 365 days / 8 workers per contractor)
        const baseDailyRatePerManpower = annualEarningsPerContractor / 365 / workersPerContractor;

        const companyBox = document.getElementById('companyBox');
        const contractorRow = document.getElementById('contractorRow');
        const btnReset = document.getElementById('btnReset');
        const btn100 = document.getElementById('btn100');
        const btn1000 = document.getElementById('btn1000');
        const totalManpowerDisplay = document.getElementById('totalManpower');
        const flowPath = document.getElementById('flowPath');

        // Company cost results elements
        const originalAnnualCompanyCostEl = document.getElementById('originalAnnualCompanyCost');
        const newAnnualCompanyCostEl = document.getElementById('newAnnualCompanyCost');
        const costPercentageIncreaseEl = document.getElementById('costPercentageIncrease');

        let totalDailyRateIncrease = 0; // This variable will store the cumulative increase from button clicks

        // Function to create a contractor box with dynamic Fitter and Welder counts
        function createContractorBox(id, numFitters, numWelders) {
            const contractorDiv = document.createElement('div');
            contractorDiv.className = 'contractor-box';
            contractorDiv.innerHTML = `
                <p>Contractor ${id}</p>
                <p class="text-sm text-gray-600">F: ${numFitters}, W: ${numWelders}</p>
                <div class="worker-group">
                    <!-- Workers will be added here -->
                </div>
                <p class="text-xs font-semibold text-gray-700 mt-2">Current Annual: <span class="current-annual-earning-value">₹0</span></p>
                <p class="text-xs font-semibold text-green-700">Annual Inc: <span class="annual-inc-value">₹0 (<span class="annual-inc-percentage">0.00</span>%)</span></p>
            `;
            const workerGroup = contractorDiv.querySelector('.worker-group');
            for (let i = 0; i < numFitters; i++) {
                const worker = document.createElement('div');
                worker.className = 'worker-icon';
                worker.textContent = 'F'; // Fitter
                workerGroup.appendChild(worker);
            }
            for (let i = 0; i < numWelders; i++) {
                const worker = document.createElement('div');
                worker.className = 'worker-icon';
                worker.textContent = 'W'; // Welder
                workerGroup.appendChild(worker);
            }
            return contractorDiv;
        }

        // Generate random distributions for Fitters and Welders for each contractor
        // ensuring total workers per contractor is 8, and at least 2 of each type.
        const contractorDistributions = [];
        for (let i = 0; i < numContractors; i++) {
            // Random Fitters between 2 and 6 (inclusive) to allow variation while meeting constraints
            const fitters = Math.floor(Math.random() * (6 - 2 + 1)) + 2;
            const welders = workersPerContractor - fitters; // Welders are the remainder to make 8
            contractorDistributions.push({ fitters, welders });
        }

        // Initialize contractor boxes (call once on page load)
        function initializeContractorBoxes() {
            contractorRow.innerHTML = ''; // Clear existing contractors
            contractorDistributions.forEach((dist, index) => {
                contractorRow.appendChild(createContractorBox(index + 1, dist.fitters, dist.welders));
            });
        }

        totalManpowerDisplay.textContent = totalManpower;

        // Function to update results and trigger animation
        function updateSimulation() {
            // Update button active states based on totalDailyRateIncrease
            // Remove active class from all buttons first
            document.querySelectorAll('.scenario-btn').forEach(btn => btn.classList.remove('active'));

            // Apply active class to the correct button
            if (totalDailyRateIncrease === 0) {
                btnReset.classList.add('active');
            } else if (totalDailyRateIncrease % 1000 === 0 && totalDailyRateIncrease !== 0) {
                btn1000.classList.add('active');
            } else {
                btn100.classList.add('active');
            }


            // Remove previous particles
            document.querySelectorAll('.particle').forEach(p => p.remove());

            const effectiveDailyRatePerManpower = baseDailyRatePerManpower + totalDailyRateIncrease;

            // Company Cost Calculations
            const originalAnnualCompanyCost = totalManpower * baseDailyRatePerManpower * 365;
            const newAnnualCompanyCost = totalManpower * effectiveDailyRatePerManpower * 365;
            let costPercentageIncrease = 0;
            if (originalAnnualCompanyCost > 0) {
                costPercentageIncrease = ((newAnnualCompanyCost / originalAnnualCompanyCost) - 1) * 100;
            }

            animateNumber(originalAnnualCompanyCostEl, originalAnnualCompanyCost);
            animateNumber(newAnnualCompanyCostEl, newAnnualCompanyCost);
            costPercentageIncreaseEl.textContent = `${costPercentageIncrease.toFixed(2)}%`;


            // Update annual earnings for each individual contractor box
            document.querySelectorAll('.contractor-box').forEach(box => {
                // Contractor's current annual earnings (with cumulative increase)
                const currentAnnualEarningForContractor = (workersPerContractor * effectiveDailyRatePerManpower) * 365;
                // Contractor's annual increase from original base rate
                const annualIncreaseFromOriginalBase = (workersPerContractor * totalDailyRateIncrease) * 365;
                // Original annual earning for this contractor (this is constant for each contractor)
                const originalAnnualEarningForContractor = (workersPerContractor * baseDailyRatePerManpower) * 365;

                let percentageIncreaseForContractor = 0;
                if (originalAnnualEarningForContractor > 0) {
                    percentageIncreaseForContractor = ((currentAnnualEarningForContractor / originalAnnualEarningForContractor) - 1) * 100;
                }

                const currentAnnualEarningSpan = box.querySelector('.current-annual-earning-value');
                const annualIncSpan = box.querySelector('.annual-inc-value');
                const annualIncPercentageSpan = box.querySelector('.annual-inc-percentage');

                if (currentAnnualEarningSpan) {
                     animateNumber(currentAnnualEarningSpan, currentAnnualEarningForContractor);
                }
                if (annualIncSpan) {
                    animateNumber(annualIncSpan, annualIncreaseFromOriginalBase);
                }
                if (annualIncPercentageSpan) {
                    annualIncPercentageSpan.textContent = percentageIncreaseForContractor.toFixed(2);
                }
            });

            // Animate flow path
            flowPath.style.height = '0px'; // Reset height
            setTimeout(() => {
                flowPath.style.height = '150px'; // Animate to a height (adjust as needed)
            }, 100);


            // Simple particle animation for money flow (trigger only if there's an increase)
            if (totalDailyRateIncrease > 0) {
                const companyRect = document.querySelector('.company-box').getBoundingClientRect();
                const contractorRects = Array.from(document.querySelectorAll('.contractor-box')).map(el => el.getBoundingClientRect());

                for (let i = 0; i < 20; i++) { // Generate some particles
                    setTimeout(() => {
                        const particle = document.createElement('div');
                        particle.className = 'particle';
                        particle.style.left = `${companyRect.left + companyRect.width / 2 - 3.5}px`; /* Center particle better */
                        particle.style.top = `${companyRect.bottom - 10}px`;
                        document.body.appendChild(particle);

                        // Randomly pick a contractor to send particle to
                        const targetContractorRect = contractorRects[Math.floor(Math.random() * contractorRects.length)];

                        // Animate particle
                        particle.style.transition = 'none'; // Disable transition for initial positioning
                        particle.offsetHeight; // Trigger reflow
                        particle.style.transition = 'opacity 0.5s ease-out, transform 1.5s ease-in-out'; // Re-enable transition

                        particle.style.opacity = 1;
                        particle.style.transform = `translate(${targetContractorRect.left + targetContractorRect.width / 2 - (companyRect.left + companyRect.width / 2)}px, ${targetContractorRect.top - companyRect.bottom + 10}px)`;

                        setTimeout(() => {
                            particle.style.opacity = 0;
                            setTimeout(() => particle.remove(), 500); // Remove after fade out
                        }, 1200);

                    }, i * 100); // Stagger particle appearance
                }
            }
        }

        // Function to animate number counting
        function animateNumber(element, targetValue) {
            let startValue = parseFloat(element.textContent.replace('₹', '').replace(/,/g, '').replace('%', '')) || 0;
            const duration = 1500; // milliseconds
            const startTime = performance.now();
            const isPercentage = element.id === 'costPercentageIncrease';

            function update(currentTime) {
                const elapsedTime = currentTime - startTime;
                const progress = Math.min(elapsedTime / duration, 1);
                const currentValue = startValue + (targetValue - startValue) * progress;

                if (isPercentage) {
                    element.textContent = `${currentValue.toFixed(2)}%`;
                } else {
                    element.textContent = `₹${Math.floor(currentValue).toLocaleString('en-IN')}`;
                }


                if (progress < 1) {
                    requestAnimationFrame(update);
                } else {
                    if (isPercentage) {
                        element.textContent = `${targetValue.toFixed(2)}%`; // Ensure final value is exact
                    } else {
                        element.textContent = `₹${Math.floor(targetValue).toLocaleString('en-IN')}`; // Ensure final value is exact
                    }
                }
            }
            requestAnimationFrame(update);
        }

        // Event listeners for buttons
        btnReset.addEventListener('click', () => {
            totalDailyRateIncrease = 0;
            updateSimulation();
        });

        btn100.addEventListener('click', () => {
            totalDailyRateIncrease += 100;
            updateSimulation();
        });

        btn1000.addEventListener('click', () => {
            totalDailyRateIncrease += 1000;
            updateSimulation();
        });

        // Initial simulation update on load
        window.onload = function() {
            initializeContractorBoxes(); // Create contractor boxes first
            updateSimulation(); // Then update simulation with initial increase (0 for reset)
        };
    </script>
</body>
</html>
