<h1 align="left">Diabetes Prediction using Machine Learning</h1>

###

<p align="left">This project aims to predict diabetes using various machine learning algorithms. The model is trained on the Pima Indians Diabetes Database and can provide predictions based on medical predictor variables.</p>

###

<div class="group/conversation-turn relative flex w-full min-w-0 flex-col agent-turn">
    <div class="flex-col gap-1 md:gap-3">
        <div class="flex flex-grow flex-col max-w-full">
            <div data-message-author-role="assistant" data-message-id="39310f81-a50d-477a-b713-f8ddc6b303d0" dir="auto"
                class="min-h-[20px] text-message flex w-full flex-col items-end gap-2 whitespace-pre-wrap break-words [.text-message+&amp;]:mt-5 overflow-x-auto">
                <div class="flex w-full flex-col gap-1 empty:hidden first:pt-[3px]">
                    <div class="markdown prose w-full break-words dark:prose-invert light">
                        <hr>
                        <h1>Diabetes Prediction using Machine Learning</h1>
                        <h2>Description</h2>
                        <p>This project aims to predict diabetes using various machine learning algorithms. The model is
                            trained on the Pima Indians Diabetes Database and can provide predictions based on medical
                            predictor variables.</p>
                        <h2>Table of Contents</h2>
                        <ul>
                            <li><a rel="noreferrer" href="#installation">Installation</a></li>
                            <li><a rel="noreferrer" href="#usage">Usage</a></li>
                            <li><a rel="noreferrer" href="#dataset">Dataset</a></li>
                            <li><a rel="noreferrer" href="#model-and-methodology">Model and Methodology</a></li>
                            <li><a rel="noreferrer" href="#results">Results</a></li>
                            <li><a rel="noreferrer" href="#contributing">Contributing</a></li>
                            <li><a rel="noreferrer" href="#license">License</a></li>
                        </ul>
                        <h2>Installation</h2>
                        <ol>
                            <li>Clone the repository:
                                <pre><div class="dark bg-gray-950 rounded-md border-[0.5px] border-token-border-medium"><div class="flex items-center relative text-token-text-secondary bg-token-main-surface-secondary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><div class="flex items-center"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24" class="icon-sm"><path fill="currentColor" fill-rule="evenodd" d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z" clip-rule="evenodd"></path></svg></button></span></div></div><div class="overflow-y-auto p-4" dir="ltr"><code class="!whitespace-pre hljs language-bash">git <span class="hljs-built_in">clone</span> https://github.com/mostafaabdoelgohary2003AI/Diabetes-Prediction.git
</code></div></div></pre>
                            </li>
                            <li>Navigate to the project directory:
                                <pre><div class="dark bg-gray-950 rounded-md border-[0.5px] border-token-border-medium"><div class="flex items-center relative text-token-text-secondary bg-token-main-surface-secondary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><div class="flex items-center"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24" class="icon-sm"><path fill="currentColor" fill-rule="evenodd" d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z" clip-rule="evenodd"></path></svg></button></span></div></div><div class="overflow-y-auto p-4" dir="ltr"><code class="!whitespace-pre hljs language-bash"><span class="hljs-built_in">cd</span> Diabetes-Prediction
</code></div></div></pre>
                            </li>
                            <li>Install the required packages:
                                <pre><div class="dark bg-gray-950 rounded-md border-[0.5px] border-token-border-medium"><div class="flex items-center relative text-token-text-secondary bg-token-main-surface-secondary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><div class="flex items-center"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24" class="icon-sm"><path fill="currentColor" fill-rule="evenodd" d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z" clip-rule="evenodd"></path></svg></button></span></div></div><div class="overflow-y-auto p-4" dir="ltr"><code class="!whitespace-pre hljs language-bash">pip install -r requirements.txt
</code></div></div></pre>
                            </li>
                        </ol>
                        <h2>Usage</h2>
                        <ol>
                            <li>Open the Jupyter Notebook:
                                <pre><div class="dark bg-gray-950 rounded-md border-[0.5px] border-token-border-medium"><div class="flex items-center relative text-token-text-secondary bg-token-main-surface-secondary px-4 py-2 text-xs font-sans justify-between rounded-t-md"><div class="flex items-center"><span class="" data-state="closed"><button class="flex gap-1 items-center"><svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24" class="icon-sm"><path fill="currentColor" fill-rule="evenodd" d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z" clip-rule="evenodd"></path></svg></button></span></div></div><div class="overflow-y-auto p-4" dir="ltr"><code class="!whitespace-pre hljs language-bash">jupyter notebook <span class="hljs-string">"Diabetes Prediction (Mostafa Abdo) in Machine Learning.ipynb"</span>
</code></div></div></pre>
                            </li>
                            <li>Follow the instructions in the notebook to run the model and make predictions.</li>
                        </ol>
                        <h2>Dataset</h2>
                        <p>The dataset used is the Pima Indians Diabetes Database from the UCI Machine Learning
                            Repository. It includes medical data such as blood pressure, insulin levels, BMI, and age,
                            among others. The target variable indicates whether a patient has diabetes.</p>
                        <h2>Model and Methodology</h2>
                        <p>The project implements multiple machine learning algorithms:</p>
                        <ul>
                            <li>Logistic Regression</li>
                            <li>Decision Trees</li>
                            <li>Random Forests</li>
                        </ul>
                        <p>The methodology involves data preprocessing, feature selection, model training, and
                            evaluation using metrics like accuracy, precision, recall, and F1 score.</p>
                        <h2>Results</h2>
                        <p>The model achieved the following metrics:</p>
                        <ul>
                            <li>Accuracy: 0.9476</li>
                            <li>Precision:<ul>
                                    <li>Class 0: 0.98</li>
                                    <li>Class 1: 0.67</li>
                                </ul>
                            </li>
                            <li>Recall:<ul>
                                    <li>Class 0: 0.96</li>
                                    <li>Class 1: 0.80</li>
                                </ul>
                            </li>
                            <li>F1 Score:<ul>
                                    <li>Class 0: 0.97</li>
                                    <li>Class 1: 0.73</li>
                                </ul>
                            </li>
                            <li>Support:<ul>
                                    <li>Class 0: 17525</li>
                                    <li>Class 1: 1701</li>
                                </ul>
                            </li>
                        </ul>
                        <p>Overall performance:</p>
                        <ul>
                            <li>Macro average F1 Score: 0.85</li>
                            <li>Weighted average F1 Score: 0.95</li>
                        </ul>
                        <h2>Contributing</h2>
                        <p>Contributions are welcome! Please open an issue or submit a pull request for any improvements
                            or additions.</p>
                        <h2>License</h2>
                        <p>This project is licensed under the MIT License. See the <a rel="noreferrer">LICENSE</a> file
                            for details.</p>
                        <hr>
                    </div>
                </div>
            </div>
        </div>
        <div class="mt-1 flex gap-3 empty:hidden -ml-2">
            <div class="items-center justify-start rounded-xl p-1 flex">
                <div class="flex items-center"><span class="" data-state="closed"><button
                            class="rounded-lg text-token-text-secondary hover:bg-token-main-surface-secondary"><span
                                class="flex h-[30px] w-[30px] items-center justify-center"><svg
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                    viewBox="0 0 24 24" class="icon-md-heavy">
                                    <path fill="currentColor" fill-rule="evenodd"
                                        d="M11 4.91a.5.5 0 0 0-.838-.369L6.676 7.737A1 1 0 0 1 6 8H4a1 1 0 0 0-1 1v6a1 1 0 0 0 1 1h2a1 1 0 0 1 .676.263l3.486 3.196A.5.5 0 0 0 11 19.09zM8.81 3.067C10.415 1.597 13 2.735 13 4.91v14.18c0 2.175-2.586 3.313-4.19 1.843L5.612 18H4a3 3 0 0 1-3-3V9a3 3 0 0 1 3-3h1.611zm11.507 3.29a1 1 0 0 1 1.355.401A10.96 10.96 0 0 1 23 12c0 1.85-.458 3.597-1.268 5.13a1 1 0 1 1-1.768-.934A8.96 8.96 0 0 0 21 12a8.96 8.96 0 0 0-1.085-4.287 1 1 0 0 1 .402-1.356M15.799 7.9a1 1 0 0 1 1.4.2 6.48 6.48 0 0 1 1.3 3.9c0 1.313-.39 2.537-1.06 3.56a1 1 0 0 1-1.673-1.096A4.47 4.47 0 0 0 16.5 12a4.47 4.47 0 0 0-.9-2.7 1 1 0 0 1 .2-1.4"
                                        clip-rule="evenodd"></path>
                                </svg></span></button></span><span class="" data-state="closed"><button
                            class="rounded-lg text-token-text-secondary hover:bg-token-main-surface-secondary"><span
                                class="flex h-[30px] w-[30px] items-center justify-center"><svg
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                    viewBox="0 0 24 24" class="icon-md-heavy">
                                    <path fill="currentColor" fill-rule="evenodd"
                                        d="M7 5a3 3 0 0 1 3-3h9a3 3 0 0 1 3 3v9a3 3 0 0 1-3 3h-2v2a3 3 0 0 1-3 3H5a3 3 0 0 1-3-3v-9a3 3 0 0 1 3-3h2zm2 2h5a3 3 0 0 1 3 3v5h2a1 1 0 0 0 1-1V5a1 1 0 0 0-1-1h-9a1 1 0 0 0-1 1zM5 9a1 1 0 0 0-1 1v9a1 1 0 0 0 1 1h9a1 1 0 0 0 1-1v-9a1 1 0 0 0-1-1z"
                                        clip-rule="evenodd"></path>
                                </svg></span></button></span><span class="" data-state="closed"><button
                            class="rounded-lg text-token-text-secondary hover:bg-token-main-surface-secondary"><span
                                class="flex h-[30px] w-[30px] items-center justify-center"><svg
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                    viewBox="0 0 24 24" class="icon-md-heavy">
                                    <path fill="currentColor"
                                        d="M3.07 10.876C3.623 6.436 7.41 3 12 3a9.15 9.15 0 0 1 6.012 2.254V4a1 1 0 1 1 2 0v4a1 1 0 0 1-1 1H15a1 1 0 1 1 0-2h1.957A7.15 7.15 0 0 0 12 5a7 7 0 0 0-6.946 6.124 1 1 0 1 1-1.984-.248m16.992 1.132a1 1 0 0 1 .868 1.116C20.377 17.564 16.59 21 12 21a9.15 9.15 0 0 1-6-2.244V20a1 1 0 1 1-2 0v-4a1 1 0 0 1 1-1h4a1 1 0 1 1 0 2H7.043A7.15 7.15 0 0 0 12 19a7 7 0 0 0 6.946-6.124 1 1 0 0 1 1.116-.868">
                                    </path>
                                </svg></span></button></span>
                    <div class="flex"><span class="" data-state="closed"><button
                                class="rounded-lg text-token-text-secondary hover:bg-token-main-surface-secondary"><span
                                    class="flex h-[30px] w-[30px] items-center justify-center"><svg
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24" class="icon-md-heavy">
                                        <path fill="currentColor" fill-rule="evenodd"
                                            d="M11.873 21.496a1 1 0 0 1-.992.496l-.454-.056A4 4 0 0 1 7.1 16.79L7.65 15h-.718c-2.637 0-4.553-2.508-3.859-5.052l1.364-5A4 4 0 0 1 8.296 2h9.709a3 3 0 0 1 3 3v7a3 3 0 0 1-3 3h-2c-.26 0-.5.14-.628.364zM14.005 4h-5.71a2 2 0 0 0-1.929 1.474l-1.363 5A2 2 0 0 0 6.933 13h2.072a1 1 0 0 1 .955 1.294l-.949 3.084a2 2 0 0 0 1.462 2.537l3.167-5.543a2.72 2.72 0 0 1 1.364-1.182V5a1 1 0 0 0-1-1m3 9V5c0-.35-.06-.687-.171-1h1.17a1 1 0 0 1 1 1v7a1 1 0 0 1-1 1z"
                                            clip-rule="evenodd"></path>
                                    </svg></span></button></span></div><span class="" data-state="closed"><button
                            type="button" id="radix-:r8a:" aria-haspopup="menu" aria-expanded="false"
                            data-state="closed"
                            class="cursor-pointer h-[30px] rounded-md px-1 text-token-text-secondary hover:bg-token-main-surface-secondary">
                            <div class="flex items-center pb-0">
                                <div class="[&amp;_svg]:h-full [&amp;_svg]:w-full icon-md h-4 w-4"><svg
                                        xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                        viewBox="0 0 24 24">
                                        <path fill="currentColor"
                                            d="M19.898.855a.4.4 0 0 0-.795 0c-.123 1.064-.44 1.802-.943 2.305-.503.503-1.241.82-2.306.943a.4.4 0 0 0 .001.794c1.047.119 1.801.436 2.317.942.512.504.836 1.241.93 2.296a.4.4 0 0 0 .796 0c.09-1.038.413-1.792.93-2.308.515-.516 1.269-.839 2.306-.928a.4.4 0 0 0 .001-.797c-1.055-.094-1.792-.418-2.296-.93-.506-.516-.823-1.27-.941-2.317Z">
                                        </path>
                                        <path fill="currentColor"
                                            d="M12.001 1.5a1 1 0 0 1 .993.887c.313 2.77 1.153 4.775 2.5 6.146 1.34 1.366 3.3 2.223 6.095 2.47a1 1 0 0 1-.003 1.993c-2.747.238-4.75 1.094-6.123 2.467-1.373 1.374-2.229 3.376-2.467 6.123a1 1 0 0 1-1.992.003c-.248-2.795-1.105-4.754-2.47-6.095-1.372-1.347-3.376-2.187-6.147-2.5a1 1 0 0 1-.002-1.987c2.818-.325 4.779-1.165 6.118-2.504 1.339-1.34 2.179-3.3 2.504-6.118A1 1 0 0 1 12 1.5ZM6.725 11.998c1.234.503 2.309 1.184 3.21 2.069.877.861 1.56 1.888 2.063 3.076.5-1.187 1.18-2.223 2.051-3.094.871-.87 1.907-1.55 3.094-2.05-1.188-.503-2.215-1.187-3.076-2.064-.885-.901-1.566-1.976-2.069-3.21-.505 1.235-1.19 2.3-2.081 3.192-.891.89-1.957 1.576-3.192 2.082Z">
                                        </path>
                                    </svg></div><svg
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                    viewBox="0 0 24 24" class="icon-sm text-token-text-quaternary">
                                    <path fill="currentColor" fill-rule="evenodd"
                                        d="M5.293 9.293a1 1 0 0 1 1.414 0L12 14.586l5.293-5.293a1 1 0 1 1 1.414 1.414l-6 6a1 1 0 0 1-1.414 0l-6-6a1 1 0 0 1 0-1.414"
                                        clip-rule="evenodd"></path>
                                </svg>
                            </div>
                        </button></span>
                </div>
            </div>
        </div>
        <div class="pr-2 lg:pr-0"></div>
        <div class="mt-3 w-full empty:hidden">
            <div class="text-center">
                <div class="mx-auto">
                    <div style="opacity: 1;">
                        <div class="inline-flex rounded-xl border border-gray-100 dark:border-gray-700">
                            <div
                                class="flex items-center justify-center gap-4 px-4 py-3 text-sm text-token-text-secondary">
                                <div class="flex items-center gap-5"><button
                                        class="text-token-text-secondary hover:text-token-text-primary"><svg
                                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                            viewBox="0 0 24 24" class="icon-md">
                                            <path fill="currentColor" fill-rule="evenodd"
                                                d="M12.132 2.504a1 1 0 0 1 .992-.496l.454.056a4 4 0 0 1 3.327 5.146L16.354 9h.718c2.638 0 4.553 2.508 3.86 5.053l-1.364 5A4 4 0 0 1 15.708 22H6a3 3 0 0 1-3-3v-7a3 3 0 0 1 3-3h2c.26 0 .5-.14.628-.364zM10 20h5.709a2 2 0 0 0 1.93-1.474l1.363-5A2 2 0 0 0 17.072 11H15a1 1 0 0 1-.956-1.294l.95-3.084a2 2 0 0 0-1.462-2.537l-3.168 5.543A2.72 2.72 0 0 1 9 10.81V19a1 1 0 0 0 1 1m-3-9v8c0 .35.06.687.17 1H6a1 1 0 0 1-1-1v-7a1 1 0 0 1 1-1z"
                                                clip-rule="evenodd"></path>
                                        </svg></button><button
                                        class="text-token-text-secondary hover:text-token-text-primary"><svg
                                            xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                            viewBox="0 0 24 24" class="icon-md">
                                            <path fill="currentColor" fill-rule="evenodd"
                                                d="M11.873 21.496a1 1 0 0 1-.992.496l-.454-.056A4 4 0 0 1 7.1 16.79L7.65 15h-.718c-2.637 0-4.553-2.508-3.859-5.052l1.364-5A4 4 0 0 1 8.296 2h9.709a3 3 0 0 1 3 3v7a3 3 0 0 1-3 3h-2c-.26 0-.5.14-.628.364zM14.005 4h-5.71a2 2 0 0 0-1.929 1.474l-1.363 5A2 2 0 0 0 6.933 13h2.072a1 1 0 0 1 .955 1.294l-.949 3.084a2 2 0 0 0 1.462 2.537l3.167-5.543a2.72 2.72 0 0 1 1.364-1.182V5a1 1 0 0 0-1-1m3 9V5c0-.35-.06-.687-.171-1h1.17a1 1 0 0 1 1 1v7a1 1 0 0 1-1 1z"
                                                clip-rule="evenodd"></path>
                                        </svg></button></div>
                            </div>
                            <div class="w-px flex-1 self-stretch bg-token-main-surface-tertiary"></div><button
                                class="text-token-text-secondary hover:text-token-text-primary p-3"><svg
                                    xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none"
                                    viewBox="0 0 24 24"
                                    class="icon-md text-token-text-secondary hover:text-token-text-primary">
                                    <path fill="currentColor" fill-rule="evenodd"
                                        d="M5.636 5.636a1 1 0 0 1 1.414 0l4.95 4.95 4.95-4.95a1 1 0 0 1 1.414 1.414L13.414 12l4.95 4.95a1 1 0 0 1-1.414 1.414L12 13.414l-4.95 4.95a1 1 0 0 1-1.414-1.414l4.95-4.95-4.95-4.95a1 1 0 0 1 0-1.414"
                                        clip-rule="evenodd"></path>
                                </svg></button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>

###
<h2 align="left">Software Used</h2>

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="40" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/numpy/numpy-original.svg" height="40" alt="numpy logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" height="40" alt="pandas logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jupyter/jupyter-original.svg" height="40" alt="jupyter logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/anaconda/anaconda-original.svg" height="40" alt="anaconda logo"  />
  <img width="12" />
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/05/Scikit_learn_logo_small.svg" height = "40" alt="sklearn logo" />
  <img width="12" />
  <img src="https://upload.wikimedia.org/wikipedia/commons/0/01/Created_with_Matplotlib-logo.svg" height = "40" alt="Matplotlib logo" />
  <img width="12" />
  <img src = "https://seaborn.pydata.org/_images/logo-tall-lightbg.svg" height="40" alt="Seaborn Logo" />
  <img width="12" />
</div>

###
