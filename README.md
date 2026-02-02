{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": []
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "source": [
        "Python Programing Basic Foundation\n",
        "\n",
        "*****1.Foundational Knowledge ****\n",
        "Differences between DataType:\n",
        "1.Lists\n",
        "2.Tuples\n",
        "3.Dictionaries\n",
        "4.Sets\n",
        "5.Conditional Statement: Learn how to apply if-else statements for decision-making.\n",
        "6.Loop: Learn how Use loops effectively for iterating over sequences.\n",
        "Understand the role of break and continue in loop control.\n"
      ],
      "metadata": {
        "id": "kjbYa1bXDiC3"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Setup and Basic Operations:"
      ],
      "metadata": {
        "id": "3aurAk9wdW4u"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "name = \"John\"\n",
        "age = 25\n",
        "print(\"Hello\", name)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "1lDeaVR9uJ1z",
        "outputId": "698ca74e-9c03-45ff-ad37-0b105d84f28c"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Hello John\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Data type means**\n",
        "Data Type = The category or kind of value that a variable can hold.\n",
        "It tells Python:\n",
        "What kind of data is stored (number, text, true/false, etc.)\n",
        "What operations can be performed on it\n",
        "How much memory to alloc\n"
      ],
      "metadata": {
        "id": "5NeI5x-Sux79"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Understand the differences between Lists, Tuples, Dictionaries, and Sets.\n",
        "Learn how to apply if-else statements for decision-making.\n",
        "Use loops effectively for iterating over sequences.\n",
        "Understand the role of break and continue in loop control.\n"
      ],
      "metadata": {
        "id": "JoOwNy8fionK"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Create a\n",
        "List Operations:\n",
        "Create a list and perform basic operations like append(), remove(), pop(), and slicing.\n",
        "Iterate over a list using loops.\n"
      ],
      "metadata": {
        "id": "WlDijTc2gpEI"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Create a List\n",
        "\n",
        "my_list = [\"apple\", \"banana\", \"cherry\", \"date\"]\n",
        "print(\"Original list:\", my_list)\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "3Xuh9jqijwfA",
        "outputId": "87254465-d770-43c7-82cc-803f948b3ea6"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original list: ['apple', 'banana', 'cherry', 'date']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: append() - Add element to end\n",
        "\n",
        "my_list.append(\"elderberry\")\n",
        "print(\"After append:\", my_list)\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "95jhG3w2k_MF",
        "outputId": "2f3ee9af-402b-4f6f-fd6b-197a766f7c39"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After append: ['apple', 'banana', 'cherry', 'date', 'elderberry']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: remove() - Remove specific element\n",
        "\n",
        "my_list.remove(\"banana\")\n",
        "print(\"After remove:\", my_list)\n",
        "\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "583L6_BylJFE",
        "outputId": "05495e69-8de6-478a-c899-08bc697fd916"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After remove: ['apple', 'cherry', 'date', 'elderberry']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: pop() - Remove element by index\n",
        "\n",
        "removed = my_list.pop()  # Removes last item\n",
        "print(\"Popped item:\", removed)\n",
        "print(\"After pop:\", my_list)\n",
        "# Output: Popped item: elderberry\n",
        "# Output: After pop: ['apple', 'cherry', 'date']\n",
        "\n",
        "my_list.pop(1)  # Remove item at index 1\n",
        "print(\"After pop(1):\", my_list)\n",
        "# Output: After pop(1): ['apple', 'date']"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "qZ3VJ2HulgwM",
        "outputId": "90403f3a-257e-4ddc-b7c5-876ba239bc3f"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Popped item: elderberry\n",
            "After pop: ['apple', 'cherry', 'date', 'elderberry']\n",
            "After pop(1): ['apple', 'date', 'elderberry']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 5: Slicing - Extract portions\n",
        "\n",
        "numbers = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]\n",
        "\n",
        "print(numbers[2:5])    # [2, 3, 4]\n",
        "print(numbers[:4])     # [0, 1, 2, 3]\n",
        "print(numbers[6:])     # [6, 7, 8, 9]\n",
        "print(numbers[-3:])    # [7, 8, 9]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "BB5th1Axlw3Y",
        "outputId": "01870795-b0b0-42c0-ad87-5857e5e27ac2"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "[2, 3, 4]\n",
            "[0, 1, 2, 3]\n",
            "[6, 7, 8, 9]\n",
            "[7, 8, 9]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 6: Iterate with Loops\n",
        "\n",
        "fruits = [\"apple\", \"cherry\", \"date\"]\n",
        "\n",
        "# For loop\n",
        "for fruit in fruits:\n",
        "    print(fruit)\n",
        "# Output:\n",
        "# apple\n",
        "# cherry\n",
        "# date\n",
        "\n",
        "# With index\n",
        "for i in range(len(fruits)):\n",
        "    print(f\"Index {i}: {fruits[i]}\")\n",
        "# Output:\n",
        "# Index 0: apple\n",
        "# Index 1: cherry\n",
        "# Index 2: date"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "AelLuT55l1L6",
        "outputId": "2e10c46b-211a-40d8-96eb-b31b2b205d77"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "apple\n",
            "cherry\n",
            "date\n",
            "Index 0: apple\n",
            "Index 1: cherry\n",
            "Index 2: date\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Tuple Operations:\n",
        "Create and access tuple elements.\n",
        "Understand the immutability of tuples.\n",
        "**Use tuple unpacking.**\n"
      ],
      "metadata": {
        "id": "5I3aUiOznxdB"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 1: Create a Tuple\n",
        "\n",
        "my_tuple = (\"red\", \"green\", \"blue\", \"yellow\")\n",
        "print(\"Original tuple:\", my_tuple)\n",
        "# Output: Original tuple: ('red', 'green', 'blue', 'yellow')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ATVPDA00n13y",
        "outputId": "5d58fd73-5dd1-457d-8d57-b4fa23770005"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original tuple: ('red', 'green', 'blue', 'yellow')\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: Access Tuple Elements\n",
        "\n",
        "# Access by index\n",
        "print(\"First element:\", my_tuple[0])      # red\n",
        "print(\"Second element:\", my_tuple[1])     # green\n",
        "print(\"Last element:\", my_tuple[-1])      # yellow\n",
        "\n",
        "# Slicing\n",
        "print(\"First 3:\", my_tuple[:3])           # ('red', 'green', 'blue')\n",
        "print(\"Last 2:\", my_tuple[-2:])           # ('blue', 'yellow')"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0W_yUbH3oFMq",
        "outputId": "7df55d26-36f3-42fa-a197-9379966110ba"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "First element: red\n",
            "Second element: green\n",
            "Last element: yellow\n",
            "First 3: ('red', 'green', 'blue')\n",
            "Last 2: ('blue', 'yellow')\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: Understand Immutability\n",
        "\n",
        "# Tuples CANNOT be changed after creation\n",
        "coordinates = (10, 20, 30)\n",
        "\n",
        "# This will cause an ERROR:\n",
        "# coordinates[0] = 15  # TypeError: 'tuple' object does not support item assignment\n",
        "\n",
        "print(\"Tuples are immutable - cannot modify elements\")\n",
        "\n",
        "# You CAN create a new tuple\n",
        "new_coordinates = (15, 20, 30)\n",
        "print(\"New tuple:\", new_coordinates)"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "OUIcSTlToJ4h",
        "outputId": "e8bc724e-ac2b-433c-b935-37825a910774"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Tuples are immutable - cannot modify elements\n",
            "New tuple: (15, 20, 30)\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: Tuple Unpacking\n",
        "\n",
        "# Unpack into variables\n",
        "person = (\"Alice\", 25, \"Engineer\")\n",
        "name, age, job = person\n",
        "\n",
        "print(\"Name:\", name)    # Alice\n",
        "print(\"Age:\", age)      # 25\n",
        "print(\"Job:\", job)      # Engineer\n",
        "\n",
        "# Unpack with * (rest of elements)\n",
        "numbers = (1, 2, 3, 4, 5)\n",
        "first, second, *rest = numbers\n",
        "\n",
        "print(\"First:\", first)       # 1\n",
        "print(\"Second:\", second)     # 2\n",
        "print(\"Rest:\", rest)         # [3, 4, 5]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "0I7J8EgzoUHg",
        "outputId": "0c3d6696-0742-452a-ea3e-b148a1229c26"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Alice\n",
            "Age: 25\n",
            "Job: Engineer\n",
            "First: 1\n",
            "Second: 2\n",
            "Rest: [3, 4, 5]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Bonus: Iterate Over Tuple\n",
        "\n",
        "colors = (\"red\", \"green\", \"blue\")\n",
        "\n",
        "for color in colors:\n",
        "    print(color)\n",
        "# Output:\n",
        "# red\n",
        "# green\n",
        "# blue"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "1AOS8AWToalR",
        "outputId": "72aa4ef7-bcb1-4dab-ce05-ef44aa6401d6"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "red\n",
            "green\n",
            "blue\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Dictionary Operations:\n",
        "Create a dictionary with key-value pairs.\n",
        "Perform operations like adding, updating, and deleting key-value pairs.\n",
        "**Iterate through a dictionary using loops**.\n"
      ],
      "metadata": {
        "id": "6YqexBBjorlP"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 1: Create a Dictionary\n",
        "\n",
        "student = {\"name\": \"Alice\", \"age\": 22, \"grade\": \"A\"}\n",
        "print(\"Original dictionary:\", student)\n",
        "# Output: Original dictionary: {'name': 'Alice', 'age': 22, 'grade': 'A'}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Bq0OO8Ppov8v",
        "outputId": "ae60bf82-6762-4176-f933-16fb5ae6b172"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original dictionary: {'name': 'Alice', 'age': 22, 'grade': 'A'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: Access Dictionary Values\n",
        "\n",
        "print(\"Name:\", student[\"name\"])        # Alice\n",
        "print(\"Age:\", student[\"age\"])          # 22\n",
        "print(\"Grade:\", student.get(\"grade\"))  # A\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "OB4jTZPTo1Th",
        "outputId": "ead4cb8c-b722-4a87-a171-89fdddf11d49"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Name: Alice\n",
            "Age: 22\n",
            "Grade: A\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: Adding Key-Value Pairs\n",
        "\n",
        "student[\"city\"] = \"New York\"\n",
        "print(\"After adding city:\", student)\n",
        "# Output: {'name': 'Alice', 'age': 22, 'grade': 'A', 'city': 'New York'}\n",
        "\n",
        "student[\"subject\"] = \"Math\"\n",
        "print(\"After adding subject:\", student)\n",
        "# Output: {'name': 'Alice', 'age': 22, 'grade': 'A', 'city': 'New York', 'subject': 'Math'}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "179agm4MpJ_p",
        "outputId": "cc0ea409-84c0-4d7d-9acd-04e585be49cf"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After adding city: {'name': 'Alice', 'age': 22, 'grade': 'A', 'city': 'New York'}\n",
            "After adding subject: {'name': 'Alice', 'age': 22, 'grade': 'A', 'city': 'New York', 'subject': 'Math'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: Updating Key-Value Pairs\n",
        "student[\"age\"] = 23\n",
        "print(\"After updating age:\", student)\n",
        "# Output: {'name': 'Alice', 'age': 23, 'grade': 'A', 'city': 'New York', 'subject': 'Math'}\n",
        "\n",
        "student.update({\"grade\": \"A+\", \"city\": \"Boston\"})\n",
        "print(\"After update():\", student)\n",
        "# Output: {'name': 'Alice', 'age': 23, 'grade': 'A+', 'city': 'Boston', 'subject': 'Math'}\n"
      ],
      "metadata": {
        "id": "Pbp_n5VPpW55"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 5: Deleting Key-Value Pairs\n",
        "\n",
        "# Using del\n",
        "del student[\"subject\"]\n",
        "print(\"After del:\", student)\n",
        "# Output: {'name': 'Alice', 'age': 23, 'grade': 'A+', 'city': 'Boston'}\n",
        "\n",
        "# Using pop()\n",
        "removed_city = student.pop(\"city\")\n",
        "print(\"Removed city:\", removed_city)  # Boston\n",
        "print(\"After pop:\", student)\n",
        "# Output: {'name': 'Alice', 'age': 23, 'grade': 'A+'}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "dF1nQXbUpj9O",
        "outputId": "2399df12-a6f8-45c6-d4f7-b0cc6a7223ce"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After del: {'name': 'Alice', 'age': 22, 'grade': 'A', 'city': 'New York'}\n",
            "Removed city: New York\n",
            "After pop: {'name': 'Alice', 'age': 22, 'grade': 'A'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 6: Iterate Through Dictionary\n",
        "\n",
        "person = {\"name\": \"John\", \"age\": 30, \"job\": \"Engineer\"}\n",
        "\n",
        "# Iterate over keys\n",
        "for key in person:\n",
        "    print(key)\n",
        "# Output: name, age, job\n",
        "\n",
        "# Iterate over values\n",
        "for value in person.values():\n",
        "    print(value)\n",
        "# Output: John, 30, Engineer\n",
        "\n",
        "# Iterate over key-value pairs\n",
        "for key, value in person.items():\n",
        "    print(f\"{key}: {value}\")\n",
        "# Output:\n",
        "# name: John\n",
        "# age: 30\n",
        "# job: Engineer"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "DOcgJAMspsLs",
        "outputId": "612c5d2c-b9ea-4029-957e-2e033150edc3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "name\n",
            "age\n",
            "job\n",
            "John\n",
            "30\n",
            "Engineer\n",
            "name: John\n",
            "age: 30\n",
            "job: Engineer\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Set Operations:\n",
        "Create a set and perform operations like union, intersection, and difference.\n",
        "Understand the uniqueness property of sets\n"
      ],
      "metadata": {
        "id": "XPMg9T50p26c"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 1: Create a Set\n",
        "\n",
        "\n",
        "my_set = {1, 2, 3, 4, 5}\n",
        "print(\"Original set:\", my_set)\n",
        "# Output: Original set: {1, 2, 3, 4, 5}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "44tn4vOhqIAE",
        "outputId": "1001158f-a1a0-4ff8-bc38-b61d26816ed3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original set: {1, 2, 3, 4, 5}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: Understand Uniqueness Property\n",
        "\n",
        "\n",
        "# Sets automatically remove duplicates\n",
        "numbers = {1, 2, 3, 2, 4, 3, 5, 1}\n",
        "print(\"Set with duplicates removed:\", numbers)\n",
        "# Output: {1, 2, 3, 4, 5}\n",
        "\n",
        "# Creating set from list with duplicates\n",
        "items = [10, 20, 10, 30, 20, 40]\n",
        "unique_items = set(items)\n",
        "print(\"Unique items:\", unique_items)\n",
        "# Output: {10, 20, 30, 40}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "RBYagwSMqMLz",
        "outputId": "b12d20f0-4f6e-454d-d56b-37ee7d8fa24d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Set with duplicates removed: {1, 2, 3, 4, 5}\n",
            "Unique items: {40, 10, 20, 30}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: Adding Elements\n",
        "\n",
        "\n",
        "fruits = {\"apple\", \"banana\", \"cherry\"}\n",
        "fruits.add(\"orange\")\n",
        "print(\"After add:\", fruits)\n",
        "# Output: {'apple', 'banana', 'cherry', 'orange'}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "DS1itN2aqShb",
        "outputId": "f25ffdc9-3487-422b-a7cb-933ffe3187d0"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After add: {'orange', 'apple', 'cherry', 'banana'}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: Union - Combine two sets\n",
        "\n",
        "\n",
        "set_a = {1, 2, 3, 4}\n",
        "set_b = {3, 4, 5, 6}\n",
        "\n",
        "union_set = set_a.union(set_b)\n",
        "print(\"Union:\", union_set)\n",
        "# Output: {1, 2, 3, 4, 5, 6}\n",
        "\n",
        "# Alternative syntax\n",
        "union_set2 = set_a | set_b\n",
        "print(\"Union (using |):\", union_set2)\n",
        "# Output: {1, 2, 3, 4, 5, 6}\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "AxDkWQ4gqYGp",
        "outputId": "71f99b6e-a748-4cf1-9d05-5bb44681792d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Union: {1, 2, 3, 4, 5, 6}\n",
            "Union (using |): {1, 2, 3, 4, 5, 6}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 5: Intersection - Common elements\n",
        "\n",
        "\n",
        "set_a = {1, 2, 3, 4}\n",
        "set_b = {3, 4, 5, 6}\n",
        "\n",
        "intersection_set = set_a.intersection(set_b)\n",
        "print(\"Intersection:\", intersection_set)\n",
        "# Output: {3, 4}\n",
        "\n",
        "# Alternative syntax\n",
        "intersection_set2 = set_a & set_b\n",
        "print(\"Intersection (using &):\", intersection_set2)\n",
        "# Output: {3, 4}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Zo7VEj_xqflx",
        "outputId": "f3d68424-0c52-4d49-a40f-616ab32312db"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Intersection: {3, 4}\n",
            "Intersection (using &): {3, 4}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 6: Difference - Elements in A but not in B\n",
        "\n",
        "\n",
        "set_a = {1, 2, 3, 4}\n",
        "set_b = {3, 4, 5, 6}\n",
        "\n",
        "difference_set = set_a.difference(set_b)\n",
        "print(\"Difference (A - B):\", difference_set)\n",
        "# Output: {1, 2}\n",
        "\n",
        "difference_set2 = set_b.difference(set_a)\n",
        "print(\"Difference (B - A):\", difference_set2)\n",
        "# Output: {5, 6}\n",
        "\n",
        "# Alternative syntax\n",
        "diff = set_a - set_b\n",
        "print(\"Difference using -:\", diff)\n",
        "# Output: {1, 2}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "ch4QmdGFqnw_",
        "outputId": "758e3dd6-991a-46f0-b6d1-642426c72aa0"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Difference (A - B): {1, 2}\n",
            "Difference (B - A): {5, 6}\n",
            "Difference using -: {1, 2}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 7: Other Useful Operations\n",
        "\n",
        "\n",
        "# Remove element\n",
        "colors = {\"red\", \"green\", \"blue\"}\n",
        "colors.remove(\"green\")\n",
        "print(\"After remove:\", colors)\n",
        "# Output: {'red', 'blue'}\n",
        "\n",
        "# Check membership\n",
        "print(\"Is 'red' in colors?\", \"red\" in colors)  # True\n",
        "\n",
        "# Set length\n",
        "print(\"Set size:\", len(colors))  # 2"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "EXwW9IQwqshH",
        "outputId": "1b6add6c-0876-4929-f5bf-33bb51a5ea33"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "After remove: {'red', 'blue'}\n",
            "Is 'red' in colors? True\n",
            "Set size: 2\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        ". Conditional Statements:\n",
        "Implement if-else conditions for decision-making.\n",
        "Use nested if-else conditions for complex logic.\n",
        "**Conditional Statements - Execution**"
      ],
      "metadata": {
        "id": "dO6JSkdmq8jH"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 1: Basic if Statement\n",
        "\n",
        "\n",
        "age = 20\n",
        "\n",
        "if age >= 18:\n",
        "    print(\"You are an adult\")\n",
        "# Output: You are an adult"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "bOYQrdO5q-Sy",
        "outputId": "8a6ae61e-e8d1-436d-c274-ed2dbcc9b130"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "You are an adult\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: if-else Statement\n",
        "\n",
        "\n",
        "temperature = 15\n",
        "\n",
        "if temperature > 25:\n",
        "    print(\"It's hot outside\")\n",
        "else:\n",
        "    print(\"It's cool outside\")\n",
        "# Output: It's cool outside"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "eo_DjWNqrKam",
        "outputId": "69fb7de1-a83f-4ddb-ff0a-9418dd121a64"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "It's cool outside\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: if-elif-else Statement\n",
        "\n",
        "\n",
        "score = 75\n",
        "\n",
        "if score >= 90:\n",
        "    print(\"Grade: A\")\n",
        "elif score >= 80:\n",
        "    print(\"Grade: B\")\n",
        "elif score >= 70:\n",
        "    print(\"Grade: C\")\n",
        "elif score >= 60:\n",
        "    print(\"Grade: D\")\n",
        "else:\n",
        "    print(\"Grade: F\")\n",
        "# Output: Grade: C"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "Lvjx2VkrrRNF",
        "outputId": "b3d172c1-798f-4e57-8e91-c9b6781509a1"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Grade: C\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: Nested if-else (Complex Logic)\n",
        "\n",
        "\n",
        "age = 25\n",
        "has_license = True\n",
        "\n",
        "if age >= 18:\n",
        "    if has_license:\n",
        "        print(\"You can drive\")\n",
        "    else:\n",
        "        print(\"You need a license to drive\")\n",
        "else:\n",
        "    print(\"You are too young to drive\")\n",
        "# Output: You can drive"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "vFV-vfUfrWQY",
        "outputId": "fa3cd0cf-4b9a-4fda-8422-e5b1095c9ae4"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "You can drive\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 5: Multiple Conditions with AND/OR\n",
        "\n",
        "\n",
        "username = \"admin\"\n",
        "password = \"1234\"\n",
        "\n",
        "# Using AND\n",
        "if username == \"admin\" and password == \"1234\":\n",
        "    print(\"Login successful\")\n",
        "else:\n",
        "    print(\"Invalid credentials\")\n",
        "# Output: Login successful\n",
        "\n",
        "# Using OR\n",
        "day = \"Saturday\"\n",
        "\n",
        "if day == \"Saturday\" or day == \"Sunday\":\n",
        "    print(\"It's the weekend!\")\n",
        "else:\n",
        "    print(\"It's a weekday\")\n",
        "# Output: It's the weekend!\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "XP5HbDRWrb1B",
        "outputId": "fbf9c70a-60a3-4869-ab82-34b7b6764eaa"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Login successful\n",
            "It's the weekend!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 6: Nested if-else - Age & Income Example\n",
        "\n",
        "\n",
        "age = 30\n",
        "income = 50000\n",
        "\n",
        "if age >= 18:\n",
        "    if income >= 30000:\n",
        "        if income >= 50000:\n",
        "            print(\"Eligible for premium loan\")\n",
        "        else:\n",
        "            print(\"Eligible for standard loan\")\n",
        "    else:\n",
        "        print(\"Income too low for loan\")\n",
        "else:\n",
        "    print(\"Age requirement not met\")\n",
        "# Output: Eligible for premium loan\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "hUaGKWN9rkFn",
        "outputId": "af639140-e1fe-449b-9b84-b71b8b32a478"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Eligible for premium loan\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 7: Real-World Example - Grade System\n",
        "\n",
        "\n",
        "attendance = 85\n",
        "exam_score = 72\n",
        "\n",
        "if attendance >= 75:\n",
        "    if exam_score >= 90:\n",
        "        print(\"Final Grade: A\")\n",
        "    elif exam_score >= 80:\n",
        "        print(\"Final Grade: B\")\n",
        "    elif exam_score >= 70:\n",
        "        print(\"Final Grade: C\")\n",
        "    else:\n",
        "        print(\"Final Grade: D\")\n",
        "else:\n",
        "    print(\"Insufficient attendance - No grade awarded\")\n",
        "# Output: Final Grade: C"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "XdLsQPUNrrsb",
        "outputId": "ae685c92-d265-46ad-e829-31353debc549"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Final Grade: C\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Looping Constructs:\n",
        "Use for loops to iterate over lists, tuples, and dictionaries.\n",
        "Use while loops for repeating tasks.\n",
        "Implement break and continue statements to control loops.\n",
        "**Looping Constructs - Execution**"
      ],
      "metadata": {
        "id": "JwepBu2dseM6"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 1: For Loop - Iterate Over List\n",
        "\n",
        "fruits = [\"apple\", \"banana\", \"cherry\"]\n",
        "\n",
        "for fruit in fruits:\n",
        "    print(fruit)\n",
        "# Output:\n",
        "# apple\n",
        "# banana\n",
        "# cherry"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "TcE7HIeJshAP",
        "outputId": "1b518b12-0dd5-4e99-8f91-b3c2c11c9368"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "apple\n",
            "banana\n",
            "cherry\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 2: For Loop - Iterate Over Tuple\n",
        "\n",
        "coordinates = (10, 20, 30, 40)\n",
        "\n",
        "for coord in coordinates:\n",
        "    print(\"Coordinate:\", coord)\n",
        "# Output:\n",
        "# Coordinate: 10\n",
        "# Coordinate: 20\n",
        "# Coordinate: 30\n",
        "# Coordinate: 40"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "nxrE8k3FtFQV",
        "outputId": "d2d40cf4-7b0e-4c56-a462-46ca7f403159"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Coordinate: 10\n",
            "Coordinate: 20\n",
            "Coordinate: 30\n",
            "Coordinate: 40\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 3: For Loop - Iterate Over Dictionary\n",
        "\n",
        "\n",
        "student = {\"name\": \"John\", \"age\": 22, \"grade\": \"A\"}\n",
        "\n",
        "# Iterate over keys\n",
        "for key in student:\n",
        "    print(key)\n",
        "# Output: name, age, grade\n",
        "\n",
        "# Iterate over values\n",
        "for value in student.values():\n",
        "    print(value)\n",
        "# Output: John, 22, A\n",
        "\n",
        "# Iterate over key-value pairs\n",
        "for key, value in student.items():\n",
        "    print(f\"{key}: {value}\")\n",
        "# Output:\n",
        "# name: John\n",
        "# age: 22\n",
        "# grade: A"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "HZ3VdF7htLlA",
        "outputId": "47573a69-4de7-4ae0-a30a-c2e3036963c4"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "name\n",
            "age\n",
            "grade\n",
            "John\n",
            "22\n",
            "A\n",
            "name: John\n",
            "age: 22\n",
            "grade: A\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 4: For Loop with range()\n",
        "\n",
        "\n",
        "# Print numbers 0 to 4\n",
        "for i in range(5):\n",
        "    print(i)\n",
        "# Output: 0, 1, 2, 3, 4\n",
        "\n",
        "# Print numbers 2 to 8\n",
        "for i in range(2, 9):\n",
        "    print(i)\n",
        "# Output: 2, 3, 4, 5, 6, 7, 8"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "QgHLRJq_tgqA",
        "outputId": "d6c7f872-fc21-451d-cd0d-6cd4545a12b2"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0\n",
            "1\n",
            "2\n",
            "3\n",
            "4\n",
            "2\n",
            "3\n",
            "4\n",
            "5\n",
            "6\n",
            "7\n",
            "8\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 5: While Loop - Repeating Tasks\n",
        "\n",
        "\n",
        "count = 1\n",
        "\n",
        "while count <= 5:\n",
        "    print(\"Count:\", count)\n",
        "    count += 1\n",
        "# Output:\n",
        "# Count: 1\n",
        "# Count: 2\n",
        "# Count: 3\n",
        "# Count: 4\n",
        "# Count: 5"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "VuJX8AgRtnOw",
        "outputId": "3806044b-79e9-45db-be2a-d726aef3929f"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Count: 1\n",
            "Count: 2\n",
            "Count: 3\n",
            "Count: 4\n",
            "Count: 5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 6: While Loop - User Input Example\n",
        "\n",
        "\n",
        "password = \"\"\n",
        "\n",
        "while password != \"python\":\n",
        "    password = input(\"Enter password: \")\n",
        "    if password != \"python\":\n",
        "        print(\"Wrong password, try again\")\n",
        "\n",
        "print(\"Access granted!\")"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "j51KNFBFt9WE",
        "outputId": "cc5df2c3-41a8-4480-c5e9-e2ba8fa11b47"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Enter password: !=\n",
            "Wrong password, try again\n",
            "Enter password: python\n",
            "Access granted!\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 7: break Statement - Exit Loop Early\n",
        "\n",
        "# Stop loop when condition is met\n",
        "for i in range(10):\n",
        "    if i == 5:\n",
        "        break\n",
        "    print(i)\n",
        "# Output: 0, 1, 2, 3, 4\n",
        "\n",
        "# While loop with break\n",
        "count = 0\n",
        "while True:\n",
        "    print(count)\n",
        "    count += 1\n",
        "    if count == 3:\n",
        "        break\n",
        "# Output: 0, 1, 2\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "rYwrwqAzuZUa",
        "outputId": "22f825bc-37da-42ae-846f-4210a237a563"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "0\n",
            "1\n",
            "2\n",
            "3\n",
            "4\n",
            "0\n",
            "1\n",
            "2\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 8: continue Statement - Skip Current Iteration\n",
        "\n",
        "\n",
        "# Skip even numbers\n",
        "for i in range(10):\n",
        "    if i % 2 == 0:\n",
        "        continue\n",
        "    print(i)\n",
        "# Output: 1, 3, 5, 7, 9\n",
        "\n",
        "# Skip specific value\n",
        "numbers = [1, 2, 3, 4, 5]\n",
        "for num in numbers:\n",
        "    if num == 3:\n",
        "        continue\n",
        "    print(num)\n",
        "# Output: 1, 2, 4, 5"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "uHE8iwJ4umKz",
        "outputId": "38304a5e-7c12-4c8b-a989-2ef584350343"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1\n",
            "3\n",
            "5\n",
            "7\n",
            "9\n",
            "1\n",
            "2\n",
            "4\n",
            "5\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 9: Combining break and continue\n",
        "\n",
        "\n",
        "# Find first number divisible by 7\n",
        "for i in range(1, 50):\n",
        "    if i % 2 == 0:\n",
        "        continue  # Skip even numbers\n",
        "    if i % 7 == 0:\n",
        "        print(\"First odd number divisible by 7:\", i)\n",
        "        break\n",
        "# Output: First odd number divisible by 7: 7"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "fK7JguKausp-",
        "outputId": "7af247bb-b905-442d-e08a-a83e34e8db50"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "First odd number divisible by 7: 7\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step 10: Nested Loops\n",
        "\n",
        "\n",
        "# Multiplication table\n",
        "for i in range(1, 4):\n",
        "    for j in range(1, 4):\n",
        "        print(f\"{i} x {j} = {i*j}\")\n",
        "    print(\"---\")\n",
        "# Output:\n",
        "# 1 x 1 = 1\n",
        "# 1 x 2 = 2\n",
        "# 1 x 3 = 3\n",
        "# ---\n",
        "# 2 x 1 = 2\n",
        "# 2 x 2 = 4\n",
        "# 2 x 3 = 6\n",
        "# ---\n",
        "# etc."
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "svXYuVKqu0BH",
        "outputId": "c0a1c45e-95b6-4a63-b89a-bca16450290c"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1 x 1 = 1\n",
            "1 x 2 = 2\n",
            "1 x 3 = 3\n",
            "---\n",
            "2 x 1 = 2\n",
            "2 x 2 = 4\n",
            "2 x 3 = 6\n",
            "---\n",
            "3 x 1 = 3\n",
            "3 x 2 = 6\n",
            "3 x 3 = 9\n",
            "---\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "**Problem-Solving Tasks**:\n",
        "Write a Python program to find the largest number in a list.\n",
        "Write a Python program to count the frequency of elements in a list.\n",
        "Create a dictionary that stores student names as keys and marks as values, then find the student with the highest marks.\n",
        "Implement a while loop to print the Fibonacci series up to a given number.\n",
        "Use a set to remove duplicate elements from a list.\n"
      ],
      "metadata": {
        "id": "bAb24CbiwRds"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Task 1: Find the Largest Number in a List\n"
      ],
      "metadata": {
        "id": "xdPSFROpF-5T"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# Method 1: Using max() function\n",
        "numbers = [45, 12, 78, 23, 67, 89, 34]\n",
        "\n",
        "largest = max(numbers)\n",
        "print(\"Largest number (using max()):\", largest)\n",
        "# Output: Largest number (using max()): 89"
      ],
      "metadata": {
        "id": "4uxMtpq9we18",
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "outputId": "ba46d79d-7041-4a13-f913-3f0e882d2e70"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Largest number (using max()): 89\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 2: Using a Loop (Manual Approach)\n",
        "\n",
        "\n",
        "numbers = [45, 12, 78, 23, 67, 89, 34]\n",
        "\n",
        "# Assume first number is largest\n",
        "largest = numbers[0]\n",
        "\n",
        "# Compare with each number\n",
        "for num in numbers:\n",
        "    if num > largest:\n",
        "        largest = num\n",
        "\n",
        "print(\"Largest number (using loop):\", largest)\n",
        "# Output: Largest number (using loop): 89"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "CoVxsXAqxk0E",
        "outputId": "6aa3bf6d-1a91-4a34-ef9f-20e831faaa41"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Largest number (using loop): 89\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 3: Using sorted()\n",
        "\n",
        "\n",
        "numbers = [45, 12, 78, 23, 67, 89, 34]\n",
        "\n",
        "sorted_numbers = sorted(numbers)\n",
        "largest = sorted_numbers[-1]  # Last element\n",
        "\n",
        "print(\"Largest number (using sorted):\", largest)\n",
        "# Output: Largest number (using sorted): 89"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "wSEeF-2ixpLi",
        "outputId": "8d6ebdc2-378a-4439-9ff2-d6d78b020bc7"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Largest number (using sorted): 89\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step-by-Step Explanation (Loop Method):\n",
        "\n",
        "#Create list: [45, 12, 78, 23, 67, 89, 34]\n",
        "#Loop through each number:\n",
        "\n",
        "#12 < 45 → no change\n",
        "#78 > 45 → largest = 78\n",
        "#23 < 78 → no change\n",
        "#67 < 78 → no change\n",
        "#89 > 78 → largest = 89\n",
        "#34 < 89 → no change\n",
        "\n",
        "\n",
        "#Result: 89\n",
        "\n"
      ],
      "metadata": {
        "id": "Rgcv790Rx-0e"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Task 2: Count the Frequency of Elements in a List"
      ],
      "metadata": {
        "id": "wkx22PykFscj"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "#Task 2: Count the Frequency of Elements in a List\n",
        "\n",
        "# Method 1: Using a dictionary (Manual counting)\n",
        "numbers = [1, 2, 3, 2, 4, 1, 5, 2, 3, 1, 4, 2]\n",
        "\n",
        "frequency = {}\n",
        "\n",
        "for num in numbers:\n",
        "    if num in frequency:\n",
        "        frequency[num] += 1\n",
        "    else:\n",
        "        frequency[num] = 1\n",
        "\n",
        "print(\"Frequency (using dictionary):\", frequency)\n",
        "# Output: Frequency (using dictionary): {1: 3, 2: 4, 3: 2, 4: 2, 5: 1}"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "fVV9i1DHEgdq",
        "outputId": "c3d35da4-8665-46c4-a38e-2b06c3efde28"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Frequency (using dictionary): {1: 3, 2: 4, 3: 2, 4: 2, 5: 1}\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 2: Using count() method\n",
        "\n",
        "\n",
        "numbers = [1, 2, 3, 2, 4, 1, 5, 2, 3, 1, 4, 2]\n",
        "\n",
        "# Get unique elements\n",
        "unique_numbers = set(numbers)\n",
        "\n",
        "for num in unique_numbers:\n",
        "    count = numbers.count(num)\n",
        "    print(f\"{num} appears {count} times\")\n",
        "# Output:\n",
        "# 1 appears 3 times\n",
        "# 2 appears 4 times\n",
        "# 3 appears 2 times\n",
        "# 4 appears 2 times\n",
        "# 5 appears 1 times"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "TDcmaXvrElSR",
        "outputId": "484cd631-614a-4d99-be24-1008d217e0e3"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "1 appears 3 times\n",
            "2 appears 4 times\n",
            "3 appears 2 times\n",
            "4 appears 2 times\n",
            "5 appears 1 times\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 3: Display as formatted output\n",
        "fruits = [\"apple\", \"banana\", \"apple\", \"cherry\", \"banana\", \"apple\", \"date\"]\n",
        "\n",
        "frequency = {}\n",
        "\n",
        "for fruit in fruits:\n",
        "    if fruit in frequency:\n",
        "        frequency[fruit] += 1\n",
        "    else:\n",
        "        frequency[fruit] = 1\n",
        "\n",
        "print(\"Fruit Frequency:\")\n",
        "for fruit, count in frequency.items():\n",
        "    print(f\"{fruit}: {count}\")\n",
        "# Output:\n",
        "# apple: 3\n",
        "# banana: 2\n",
        "# cherry: 1\n",
        "# date: 1"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "BDNsM8IlElN_",
        "outputId": "cf0b1147-71de-4233-c585-a6fcfae88174"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Fruit Frequency:\n",
            "apple: 3\n",
            "banana: 2\n",
            "cherry: 1\n",
            "date: 1\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#fruits = [\"apple\", \"banana\", \"apple\", \"cherry\", \"banana\", \"apple\", \"date\"]\n",
        "\n",
        "#frequency = {}\n",
        "\n",
        "#for fruit in fruits:\n",
        "    #if fruit in frequency:\n",
        "        #frequency[fruit] += 1\n",
        "    #else:\n",
        "        #frequency[fruit] = 1\n",
        "\n",
        "#print(\"Fruit Frequency:\")\n",
        "#for fruit, count in frequency.items():\n",
        "    #print(f\"{fruit}: {count}\")\n",
        "# Output:\n",
        "# apple: 3\n",
        "# banana: 2\n",
        "# cherry: 1\n",
        "# date: 1"
      ],
      "metadata": {
        "id": "LTP3kAA9E3I5"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Task 3: Student Marks Dictionary - Find Highest Marks\n"
      ],
      "metadata": {
        "id": "1vfjGbDFFklz"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# Method 1: Using max() with dictionary values\n",
        "students = {\n",
        "    \"Alice\": 85,\n",
        "    \"Bob\": 92,\n",
        "    \"Charlie\": 78,\n",
        "    \"Diana\": 95,\n",
        "    \"Eve\": 88\n",
        "}\n",
        "\n",
        "# Find student with highest marks\n",
        "highest_marks = max(students.values())\n",
        "top_student = max(students, key=students.get)\n",
        "\n",
        "print(\"Highest marks:\", highest_marks)\n",
        "print(\"Top student:\", top_student)\n",
        "# Output:\n",
        "# Highest marks: 95\n",
        "# Top student: Diana"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "3AOnR367GNPR",
        "outputId": "990c24fc-4118-403a-b237-fb0edd872ddf"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Highest marks: 95\n",
            "Top student: Diana\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 2: Using a loop (Manual approach)\n",
        "\n",
        "\n",
        "students = {\n",
        "    \"Alice\": 85,\n",
        "    \"Bob\": 92,\n",
        "    \"Charlie\": 78,\n",
        "    \"Diana\": 95,\n",
        "    \"Eve\": 88\n",
        "}\n",
        "\n",
        "# Initialize with first student\n",
        "top_student = \"\"\n",
        "highest_marks = 0\n",
        "\n",
        "for name, marks in students.items():\n",
        "    if marks > highest_marks:\n",
        "        highest_marks = marks\n",
        "        top_student = name\n",
        "\n",
        "print(f\"Top student: {top_student}\")\n",
        "print(f\"Highest marks: {highest_marks}\")\n",
        "# Output:\n",
        "# Top student: Diana\n",
        "# Highest marks: 95"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "1T4kGRsQGVYs",
        "outputId": "822c1b03-05fd-4a6d-b96f-7d096bc0f98e"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Top student: Diana\n",
            "Highest marks: 95\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 3: Complete display with all students\n",
        "\n",
        "\n",
        "students = {\n",
        "    \"Alice\": 85,\n",
        "    \"Bob\": 92,\n",
        "    \"Charlie\": 78,\n",
        "    \"Diana\": 95,\n",
        "    \"Eve\": 88\n",
        "}\n",
        "\n",
        "print(\"All Students and Marks:\")\n",
        "for name, marks in students.items():\n",
        "    print(f\"{name}: {marks}\")\n",
        "\n",
        "print(\"\\n\" + \"=\"*30)\n",
        "\n",
        "# Find top student\n",
        "top_student = max(students, key=students.get)\n",
        "highest_marks = students[top_student]\n",
        "\n",
        "print(f\"🏆 Top Student: {top_student}\")\n",
        "print(f\"📊 Highest Marks: {highest_marks}\")\n",
        "\n",
        "# Output:\n",
        "# All Students and Marks:\n",
        "# Alice: 85\n",
        "# Bob: 92\n",
        "# Charlie: 78\n",
        "# Diana: 95\n",
        "# Eve: 88\n",
        "# ==============================\n",
        "# 🏆 Top Student: Diana\n",
        "# 📊 Highest Marks: 95"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "zY2pjrLgGdX0",
        "outputId": "cd9609d1-825d-4245-a216-ffc2142c4501"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "All Students and Marks:\n",
            "Alice: 85\n",
            "Bob: 92\n",
            "Charlie: 78\n",
            "Diana: 95\n",
            "Eve: 88\n",
            "\n",
            "==============================\n",
            "🏆 Top Student: Diana\n",
            "📊 Highest Marks: 95\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Step-by-Step Explanation (Loop Method):\n",
        "#Dictionary: {\"Alice\": 85, \"Bob\": 92, \"Charlie\": 78, \"Diana\": 95, \"Eve\": 88}\n",
        "\n",
        "#Initialize: top_student = \"\", highest_marks = 0\n",
        "#Loop through each student:\n",
        "\n",
        "#Alice: 85 > 0 → top_student = \"Alice\", highest_marks = 85\n",
        "#Bob: 92 > 85 → top_student = \"Bob\", highest_marks = 92\n",
        "#Charlie: 78 < 92 → no change\n",
        "#Diana: 95 > 92 → top_student = \"Diana\", highest_marks = 95\n",
        "#Eve: 88 < 95 → no change\n",
        "\n",
        "\n",
        "#Final Result: Diana with 95 marks\n",
        "\n",
        "\n",
        "#Task 3 complete! ✓\n",
        "#Ready for Task 4? Sonnet 4.5"
      ],
      "metadata": {
        "id": "0qvcuMUFGorw"
      },
      "execution_count": null,
      "outputs": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "Task 4: Fibonacci Series Using While Loop\n"
      ],
      "metadata": {
        "id": "IP-ILk9hHoLi"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# Method 1: Print Fibonacci series up to a given number\n",
        "limit = 50\n",
        "\n",
        "a = 0\n",
        "b = 1\n",
        "\n",
        "print(\"Fibonacci series up to\", limit)\n",
        "print(a, end=\" \")\n",
        "\n",
        "while b <= limit:\n",
        "    print(b, end=\" \")\n",
        "    a, b = b, a + b\n",
        "\n",
        "print()  # New line\n",
        "# Output: Fibonacci series up to 50\n",
        "# 0 1 1 2 3 5 8 13 21 34"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "F0PcrLcXH5sa",
        "outputId": "e6274d2c-74a7-4d94-c43b-2cc8eb12af8d"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Fibonacci series up to 50\n",
            "0 1 1 2 3 5 8 13 21 34 \n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 2: Print first N terms of Fibonacci\n",
        "\n",
        "\n",
        "# Print first 10 Fibonacci numbers\n",
        "n = 10\n",
        "\n",
        "a = 0\n",
        "b = 1\n",
        "count = 0\n",
        "\n",
        "print(f\"First {n} Fibonacci numbers:\")\n",
        "\n",
        "while count < n:\n",
        "    print(a, end=\" \")\n",
        "    a, b = b, a + b\n",
        "    count += 1\n",
        "\n",
        "print()\n",
        "# Output: First 10 Fibonacci numbers:\n",
        "# 0 1 1 2 3 5 8 13 21 34"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "X2Ebc1eCH-H-",
        "outputId": "3e09ffd3-f16e-4233-8b35-5006ebd57da9"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "First 10 Fibonacci numbers:\n",
            "0 1 1 2 3 5 8 13 21 34 \n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 3: Store in a list\n",
        "\n",
        "\n",
        "# Store Fibonacci numbers up to limit in a list\n",
        "limit = 100\n",
        "fibonacci_list = []\n",
        "\n",
        "a = 0\n",
        "b = 1\n",
        "\n",
        "fibonacci_list.append(a)\n",
        "\n",
        "while b <= limit:\n",
        "    fibonacci_list.append(b)\n",
        "    a, b = b, a + b\n",
        "\n",
        "print(\"Fibonacci list:\", fibonacci_list)\n",
        "# Output: Fibonacci list: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "gyvXDszoIEfX",
        "outputId": "8e198b88-36dd-49fa-eb81-a5562d75e5df"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Fibonacci list: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Store Fibonacci numbers up to limit in a list\n",
        "limit = 100\n",
        "fibonacci_list = []\n",
        "\n",
        "a = 0\n",
        "b = 1\n",
        "\n",
        "fibonacci_list.append(a)\n",
        "\n",
        "while b <= limit:\n",
        "    fibonacci_list.append(b)\n",
        "    a, b = b, a + b\n",
        "\n",
        "print(\"Fibonacci list:\", fibonacci_list)\n",
        "# Output: Fibonacci list: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89]"
      ],
      "metadata": {
        "id": "ZjrN7p7EINY1"
      }
    },
    {
      "cell_type": "markdown",
      "source": [
        "Task 5: Remove Duplicates from List Using Set"
      ],
      "metadata": {
        "id": "ta1RuYTEIeaI"
      }
    },
    {
      "cell_type": "code",
      "source": [
        "# Method 1: Convert to set and back to list\n",
        "numbers = [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "\n",
        "print(\"Original list:\", numbers)\n",
        "\n",
        "# Remove duplicates using set\n",
        "unique_numbers = list(set(numbers))\n",
        "\n",
        "print(\"List after removing duplicates:\", unique_numbers)\n",
        "# Output:\n",
        "# Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "# List after removing duplicates: [1, 2, 3, 4, 5, 6, 7]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "DqxwB0VtIfyt",
        "outputId": "8ff72217-62ec-4594-a8ba-00d548fbf4cc"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
            "List after removing duplicates: [1, 2, 3, 4, 5, 6, 7]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 2: Preserve original order\n",
        "\n",
        "\n",
        "# Using dict.fromkeys() to maintain order\n",
        "numbers = [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "\n",
        "print(\"Original list:\", numbers)\n",
        "\n",
        "# Remove duplicates while preserving order\n",
        "unique_numbers = list(dict.fromkeys(numbers))\n",
        "\n",
        "print(\"Unique list (order preserved):\", unique_numbers)\n",
        "# Output:\n",
        "# Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "# Unique list (order preserved): [1, 2, 3, 4, 5, 6, 7]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "m2yuw0E1Imoh",
        "outputId": "1d229817-40d7-4def-b265-740cba24aae6"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
            "Unique list (order preserved): [1, 2, 3, 4, 5, 6, 7]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 3: With strings/text\n",
        "\n",
        "# Remove duplicate words\n",
        "words = [\"apple\", \"banana\", \"apple\", \"cherry\", \"banana\", \"date\", \"apple\"]\n",
        "\n",
        "print(\"Original list:\", words)\n",
        "\n",
        "unique_words = list(set(words))\n",
        "\n",
        "print(\"Unique words:\", unique_words)\n",
        "# Output:\n",
        "# Original list: ['apple', 'banana', 'apple', 'cherry', 'banana', 'date', 'apple']\n",
        "# Unique words: ['banana', 'date', 'cherry', 'apple']\n"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "24lEWHfCItNq",
        "outputId": "a9a13e92-7e6a-4265-cee4-ea9b0f8d01f5"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original list: ['apple', 'banana', 'apple', 'cherry', 'banana', 'date', 'apple']\n",
            "Unique words: ['date', 'apple', 'cherry', 'banana']\n"
          ]
        }
      ]
    },
    {
      "cell_type": "code",
      "source": [
        "#Method 4: Manual approach using loop\n",
        "\n",
        "\n",
        "# Remove duplicates manually without using set\n",
        "numbers = [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "\n",
        "unique_numbers = []\n",
        "\n",
        "for num in numbers:\n",
        "    if num not in unique_numbers:\n",
        "        unique_numbers.append(num)\n",
        "\n",
        "print(\"Original list:\", numbers)\n",
        "print(\"Unique list (manual):\", unique_numbers)\n",
        "# Output:\n",
        "# Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "# Unique list (manual): [1, 2, 3, 4, 5, 6, 7]"
      ],
      "metadata": {
        "colab": {
          "base_uri": "https://localhost:8080/"
        },
        "id": "1d3xP0_kI2_b",
        "outputId": "ce9fe54e-7955-46e4-bf10-cae4b84e07ba"
      },
      "execution_count": null,
      "outputs": [
        {
          "output_type": "stream",
          "name": "stdout",
          "text": [
            "Original list: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
            "Unique list (manual): [1, 2, 3, 4, 5, 6, 7]\n"
          ]
        }
      ]
    },
    {
      "cell_type": "markdown",
      "source": [
        "Step-by-Step Explanation (Set Method):\n",
        "Original List: [1, 2, 3, 2, 4, 1, 5, 3, 6, 4, 2, 7]\n",
        "\n",
        "Convert to set: {1, 2, 3, 4, 5, 6, 7}\n",
        "\n",
        "Sets automatically remove duplicates\n",
        "Sets only keep unique values\n",
        "\n",
        "\n",
        "Convert back to list: [1, 2, 3, 4, 5, 6, 7]\n",
        "Result: All duplicates removed!\n",
        "\n"
      ],
      "metadata": {
        "id": "-gf6U6thI9rN"
      }
    }
  ]
}
