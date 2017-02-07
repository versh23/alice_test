<?php

namespace AppBundle\Entity;

use Doctrine\ORM\Mapping as ORM;

/**
 * Company
 *
 * @ORM\Table(name="company")
 * @ORM\Entity(repositoryClass="AppBundle\Repository\CompanyRepository")
 */
class Company
{
    /**
     * @var int
     *
     * @ORM\Column(name="id", type="integer")
     * @ORM\Id
     * @ORM\GeneratedValue(strategy="AUTO")
     */
    private $id;

    /**
     * @ORM\ManyToOne(targetEntity="AppBundle\Entity\Industry", cascade={"persist", "remove"})
     */
    private $industry;

    /**
     * Get id
     *
     * @return int
     */
    public function getId()
    {
        return $this->id;
    }

    /**
     * Set industry
     *
     * @param \AppBundle\Entity\Industry $industry
     *
     * @return Company
     */
    public function setIndustry(\AppBundle\Entity\Industry $industry = null)
    {
        $this->industry = $industry;

        return $this;
    }

    /**
     * Get industry
     *
     * @return \AppBundle\Entity\Industry
     */
    public function getIndustry()
    {
        return $this->industry;
    }
}
