<h1 align="center">
    🍝 Philosophers 🤓
</h1>

<p align="center">
	<b><i>Development repo for 42cursus' philosophers project</i></b><br>
	For further information about 42cursus and its projects, please refer to <a href="https://github.com/iker-gonzalez/42_cursus"><b>42cursus repo</b></a>.
</p>

<p align="center">
	<img alt="GitHub code size in bytes" src="https://img.shields.io/github/languages/code-size/iker-gonzalez/philosophers?color=blueviolet" />
	<img alt="Number of lines of code" src="https://img.shields.io/tokei/lines/github/iker-gonzalez/philosophers?color=blueviolet" />
	<img alt="Code language count" src="https://img.shields.io/github/languages/count/iker-gonzalez/philosophers?color=blue" />
	<img alt="GitHub top language" src="https://img.shields.io/github/languages/top/iker-gonzalez/philosophers?color=blue" />
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/iker-gonzalez/philosophers?color=brightgreen" />
</p>

<h3 align="center">
	<a href="#%EF%B8%8F-about">About</a>
	<span> · </span>
	<a href="#%EF%B8%8F-usage">Usage</a>
</h3>

---

## 🗣️ About

> In this project, you will learn the basics of threading a process. You will learn how to make threads. You will discover the mutex.


42's take on the classic [Dining philosophers problem](https://en.wikipedia.org/wiki/Dining_philosophers_problem). The mandatory part was done using the phtread API to execute n numbers of threads at once that eat, sleep, then start eating again. Mutex was used to manage the limited resources available.
Given the right parameters, philosophers keep repeating their cycle virtually forever, unless a maximum number of times each philosopher must eat before the simulation ends is given.
Examples:

```
n_philosophers  time_before_death time_eat  time_sleep  [time_eats]
4 410 200 200
5 800 200 200 5
```

For detailed information, refer to the [**subject of this project**](https://github.com/iker-gonzalez/42_cursus/blob/main/_PDFs/en.subject_philosophers.pdf)

 ## 🛠️ Usage

Clone the repo and open the corresponding folder.

Compile the program
```
make
```
Execute program with parameters: `n_philosophers time_before_death time_eat time_sleep [numbers_of_eats]` (last parameter is optional)
```
./philo 4 410 200 200 1
```
Expected output:
```
0 1 has taken a fork
0 1 has taken a fork
0 1 is eating
0 3 has taken a fork
0 3 has taken a fork
0 3 is eating
200 3 is sleeping
200 1 is sleeping
200 2 has taken a fork
200 2 has taken a fork
200 4 has taken a fork
200 4 has taken a fork
200 4 is eating
200 2 is eating
```
